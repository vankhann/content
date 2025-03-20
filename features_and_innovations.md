| Feature                             | Description |
|-------------------------------------|-------------|
| **Disaggregated Prefill & Decode Inference** | Separates prefill and decode stages to maximize GPU performance, balancing throughput and latency. |
| **Dynamic GPU Scheduling**          | Implements dynamic scheduling based on demand, ensuring optimal performance across variable workloads. |
| **LLM-Aware Request Routing**       | Employs smart routing for LLMs, minimizing KV cache recomputation to improve latency. |
| **Accelerated Asynchronous Data Transfer** | Facilitates high-speed asynchronous data transfer between GPUs, leveraging the NIXL library. |
| **KV Cache Offloading**             | Offloads KV cache to different memory levels, including CPU, local storage, and network storage, supporting petabytes of data. |
