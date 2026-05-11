# Ailiance

**EU-sovereign AI infrastructure.** OpenAI-compatible gateway with hardware-specialist LoRA routing. Open core, self-hosted, GDPR-ready.

🌐 [ailiance.fr](https://ailiance.fr) — [@ailiance](https://github.com/ailiance) on GitHub — [Ailiance-fr](https://huggingface.co/Ailiance-fr) on HuggingFace

---

## Why Ailiance

Most LLM stacks send your requests to US-hosted services. Ailiance is a **drop-in OpenAI-compatible gateway** that routes each prompt to the most adapted European or Swiss foundation model — Apertus 70B, Mistral Medium, EuroLLM 22B, Gemma 3 — and specialises responses through **13 hardware-domain LoRA adapters** (KiCad, STM32, SPICE, EMC, embedded, FreeCAD, DSP, IoT, power, PlatformIO, components-review, coder).

EU AI Act Art. 52/53 transparency by design. Every call leaves a JSONL audit trail. Datasets ship with full provenance (Stack Exchange CC-BY-SA, KiCad copyleft, in-house permissive).

---

## Stack at a glance

| Repo | Role |
|------|------|
| [`ailiance`](https://github.com/ailiance/ailiance) | Gateway — FastAPI router :9300, Jina v3 + MLP domain classifier, 24 aliases, EU AI Act tracing |
| [`ailiance-agent`](https://github.com/ailiance/ailiance-agent) | VS Code extension + Ink CLI (`aki`) — autonomous coding agent routed to ailiance by default |
| [`ailiance-demo`](https://github.com/ailiance/ailiance-demo) | Frontend cockpit (React 19 + FastAPI) + Tailscale admin |
| [`ailiance-mac-tuner`](https://github.com/ailiance/ailiance-mac-tuner) | MLX fine-tuning toolkit on Mac Studio M3 Ultra (512 GB) — distill Claude Opus into Mistral Large 123B |
| [`ailiance-models-tuning`](https://github.com/ailiance/ailiance-models-tuning) | Unsloth/PEFT fine-tuning pipeline for 10 hardware-expert domains on Qwen 2.5-32B |
| [`ailiance-bench`](https://github.com/ailiance/ailiance-bench) | MLX benchmarking — gsm8k, ARC, MMLU-Pro, 5-niche perplexity, base vs LoRA comparisons |

All repos are licensed under **Apache-2.0**.

---

## HuggingFace presence

- **10 production LoRA adapters** under [`clemsail/ailiance-*-sft`](https://huggingface.co/clemsail) — KiCad, STM32, SPICE, EMC, embedded, FreeCAD, DSP, IoT, power, PlatformIO. Apache-2.0.
- **10 base / specialist models** under [`Ailiance-fr/`](https://huggingface.co/Ailiance-fr) — Devstral, Apertus, EuroLLM LoRAs + 2 MiniLM domain routers. Apache-2.0.
- **13 datasets** under [`Ailiance-fr/`](https://huggingface.co/datasets/Ailiance-fr) — 11 mascarade-X-dataset (electronics Q&A) + KiCad9+ permissive/copyleft + Kill_LIFE embedded QA. CC-BY-SA-4.0 / GPL-3.0 per upstream requirements (Stack Exchange, KiCad GPL).

---

## Status

`active development` · `pre-launch` · domain `ailiance.fr` verified 2026-05-11 · 6 GitHub repos · 20 HF models · 13 HF datasets · 1.0 release pending.

For questions: `contact@ailiance.fr` · For security: `security@ailiance.fr` (or open a private security advisory on any repo).
