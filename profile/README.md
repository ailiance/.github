# Ailiance

**EU-sovereign AI infrastructure.** OpenAI-compatible gateway with domain-specialist LoRA routing. Open core, self-hosted, GDPR-ready.

🌐 [ailiance.fr](https://ailiance.fr) · [@ailiance](https://github.com/ailiance) on GitHub · [Ailiance-fr](https://huggingface.co/Ailiance-fr) on Hugging Face

---

## Why Ailiance

Most LLM stacks send your requests to US-hosted services. Ailiance is a **drop-in OpenAI-compatible gateway** that classifies each prompt with a lightweight on-device router (all-MiniLM-L6-v2 + MLP head) and dispatches it to the most adapted European or Swiss foundation model — then specialises the answer through **domain-expert LoRA adapters** (KiCad, STM32, SPICE, EMC, embedded, DSP, IoT, power, PlatformIO, FreeCAD, code, web…), hot-swapped on a sovereign Apple-Silicon + RTX cluster.

EU AI Act Art. 52/53 transparency by design. Every call leaves a JSONL audit trail. Datasets ship with full provenance (Stack Exchange CC-BY-SA, KiCad copyleft, in-house permissive).

---

## Stack at a glance

| Repo | Role |
|------|------|
| [`ailiance`](https://github.com/ailiance/ailiance) | The gateway — FastAPI router, MiniLM + MLP domain classifier, multi-LoRA hot-swap routing, OpenAI-compatible `/v1` surface, EU AI Act JSONL tracing. |
| [`isaac-cli`](https://github.com/ailiance/isaac-cli) | **ISAAC** — sovereign autonomous coding agent. VS Code extension + Ink CLI (`isaac`), routed to the gateway by default, AI-Act-compliant tracing. |
| [`ailiance-demo`](https://github.com/ailiance/ailiance-demo) | Frontend cockpit for the LLM fleet — React 19 + FastAPI, Tailscale-only admin. |
| [`iact-bench`](https://github.com/ailiance/iact-bench) | EU AI Act audit-grade benchmark — 31 domains, sandboxed Docker / MCP / KiKit validators, NDJSON audit trail. |
| [`ailiance-mac-tuner`](https://github.com/ailiance/ailiance-mac-tuner) | MLX fine-tuning toolkit for Mac Studio M3 Ultra (512 GB). |
| [`ailiance-models-tuning`](https://github.com/ailiance/ailiance-models-tuning) | Unsloth / PEFT pipeline — domain-expert LoRA adapters on Qwen3-4B-Instruct. |
| [`ailiance-bench`](https://github.com/ailiance/ailiance-bench) | MLX benchmarking — gsm8k, ARC, MMLU-Pro, base vs LoRA comparisons. |

Also in the org: `mcp-ailiance`, `ailiance-omlx-node`, `ailiance-gaia-x`, `isaac-rust`, `ailiance-coder`. All repos licensed under **Apache-2.0**.

---

## Hugging Face presence

- **10 production LoRA adapters** under [`clemsail/ailiance-*-sft`](https://huggingface.co/clemsail) — KiCad, STM32, SPICE, EMC, embedded, FreeCAD, DSP, IoT, power, PlatformIO. Apache-2.0.
- **Base / specialist models + datasets** under [`Ailiance-fr`](https://huggingface.co/Ailiance-fr) — 10 models + 13 datasets. Models Apache-2.0; datasets CC-BY-SA-4.0 / GPL-3.0 per upstream requirements (Stack Exchange, KiCad GPL).

---

## Status

`active development` · `pre-launch` · domain `ailiance.fr` verified 2026-05-11 · ~16 GitHub repos · 20 HF models · 13 HF datasets · 1.0 release pending.

For questions: `contact@ailiance.fr` · For security: `security@ailiance.fr` (or open a private security advisory on any repo).
