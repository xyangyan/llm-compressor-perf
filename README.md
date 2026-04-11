# cperf

> *Compress once, perform forever.*

**cperf** (compressor-perf) is a production-ready model compression and performance optimization toolkit.

- 🔧 **Compression** — Pruning, quantization, distillation
- ⚡ **Latency** — Kernel fusion, memory reuse, low-latency inference
- 🚀 **Throughput** — Dynamic batching, pipeline parallelism, high concurrency

---

## Quick Start

```bash
pip install compressor-perf

cperf compress model.onnx --prune 0.3
cperf quantize model --int8
cperf bench --model model.onnx --throughput
cperf serve model.onnx --port 8080 --batch 32
