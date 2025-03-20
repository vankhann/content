| Component                                      | Function |
|------------------------------------------------|----------|
| **NVIDIA Dynamo Planner**                      | Optimizes GPU resource allocation, monitors capacity metrics, and adapts to workloads. |
| **NVIDIA Dynamo Smart Router**                 | Reduces KV cache recomputation using a Radix Tree structure, achieving a **2x TTFT speedup** and **2x average latency reduction**. Results were verified on **2 HGX-H100 nodes** running **8x DeepSeek-R1-Distill-Llama-70B** with **vLLM, FP8, tensor parallelism 2**, **100K real requests**, with an average **ISL/OSL of 4K/800**. |
| **NVIDIA Dynamo Distributed KV Cache Manager** | Manages offloading KV cache to **CPU, local storage, or network storage**, supporting **petabytes of data**, and is compatible with **PyTorch, SGLang, TensorRT-LLM, vLLM**, utilizing **NVLink, Quantum, and Spectrum**. |
| **NVIDIA Inference Transfer Library (NIXL)**   | Offers a **high-performance, low-latency communication library**, supporting **GPUDirect Storage, UCX, S3**, and is available at [NIXL GitHub](https://github.com/ai-dynamo/nixl). |
