# Local Setup

1. Download [quantized](https://huggingface.co/unsloth/Qwen3.6-27B-GGUF/tree/main) models and mmproj

You can fit Q2_K_XL on 16GB VRAM with q4_0 kv cache. Generation speed is ~45 tok / s.

3. Run [llamacpp](https://github.com/ggml-org/llama.cpp/releases) on Windows host

```bash
./llama-b8913-bin-win-cuda-13.1-x64/llama-server.exe --models-preset models.ini --models-max 1 --host 0.0.0.0 --port 11434
```

3. Run opencode on WSL

```bash
opencode
```
