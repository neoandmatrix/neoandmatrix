### Hi, I'm Tushar 👋

I build **real-time voice AI** for Indian languages: speech-to-text, text-to-speech and phone agents. I like going down
to the GPU kernel level to make them fast on cheap hardware. Before that I worked as a backend engineer, mostly in
Go, Python and TypeScript.

#### Voice AI

- **[rumik-fast](https://github.com/neoandmatrix/rumik-fast):** I wrote my own inference engine for a 3B Hindi/English text-to-speech model.
  - **It runs in real time on a 4 GB laptop GPU (RTX 3050):** 59 → 95–98 tokens/s, with first sound in about 0.5 s.
  - Under the hood: int4 weights, hand-written CUDA int4 GEMV kernels, fused Triton decode, flash-decoding and streaming Mimi decoding.
  - The int4 weights are on Hugging Face: [bringagi/rumik-oss-1-int4](https://huggingface.co/bringagi/rumik-oss-1-int4).
- **[gemma-stt-hindi](https://github.com/neoandmatrix/gemma-stt-hindi):** a Hindi speech-to-text model built on Google's EmbeddingGemma 2 audio encoder, with a CTC head and a KenLM decoder.
  - It reaches **5.4% CER on Lahaja**, on par with Qwen3-ASR-1.7B.
  - It was trained on free Kaggle T4 GPUs.
  - The model is on Hugging Face: [bringagi/gemma-stt-hindi](https://huggingface.co/bringagi/gemma-stt-hindi).

#### Backend and systems

- **[rce-go](https://github.com/neoandmatrix/rce-go):** a remote code execution service written in Go.
- **[http-from-scratch](https://github.com/neoandmatrix/http-from-scratch):** HTTP/1.x implemented from scratch in Go, to learn how it works underneath.
- **[anymemory](https://github.com/neoandmatrix/anymemory):** a service for creating and storing persistent memories.
- **[terminal-todo](https://github.com/neoandmatrix/terminal-todo):** a small terminal todo app, in Go.

#### Now

- Working on a Hindi/Hinglish end-of-turn detector, on-device Indic speech recognition, and a benchmarking harness
  for GPU kernels.
- **Looking for roles in voice AI, inference optimization or backend.** Reach me at tusharannand@gmail.com.
