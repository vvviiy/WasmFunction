# WasmFunction
WasmFunction is a Kubernetes-native serverless FaaS solution built on top of WebAssembly.

![image](https://github.com/user-attachments/assets/679526d6-8360-4865-b6f7-8d46f9340c8d)

We focuses on:

Seamlessly using WebAssembly in Kubernetes like OCI Container
Reduce Kubernetes container cold start time
Build a WebAssembly-based FaaS platform on top of the optimized Kubernetes
Our solution aims to achieve comparable cold start performance without container pre-warming.


Contributing
Out solution involves development and optimization of projects and applications at different levels.

1999huye1104/wasm-faas. Made some extension and customization from fission/fission, to manage WebAssembly functions.

WasmFunction/k3s-k8s. Made some optimization about timers and reduced cold start time.

WasmFunction/containerd. Made some optimization about pod sandbox and status reporting.

WasmFunction/kuasar. Made some customization for wasm-sandboxer from the kuasar-io/kuasar, to use our external WebAssembly runtime instead.

WasmFunction/rust-extensions. Stable dependency for WasmFunction/kuasar. fixed and completed metric collecting.

WasmFunction/wasmkeeper. Customized WebAssembly runtime and also a HTTP server that serves WebAssembly function. Called by WasmFunction/kuasar and runs as the container process.

You can try it out by following steps from K8s-files/how-to-setup.md to set up the environment.

References
https://www.infracloud.io/serverless-functions-kubernetes/
https://knative.dev/docs/
https://openwhisk.apache.org/
https://www.openfaas.com/pricing/
https://cn.serverless.com/
https://kuasar.io/
