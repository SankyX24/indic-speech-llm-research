# indic-speech-llm-research
Hindi Speech-to-LLM Pipeline using Whisper Small and Qwen2.5 with ASR evaluation, noise robustness, and repetition-aware clarification.

## Project Overview

This project investigates the reliability and performance of a Hindi speech-to-text-response pipeline integrating Whisper Small for automatic speech recognition and Qwen2.5-1.5B-Instruct for language generation.

The system is evaluated on 100 Hindi speech examples, measuring word error rate (WER), character error rate (CER), inference latency, and real-time factor (RTF). Additional experiments examine acoustic noise robustness and the impact of spectral denoising.

A repetition-aware transcript quality gate is introduced to detect degenerate ASR outputs and selectively request clarification rather than generate potentially unreliable responses. The proposed mechanism flags 8% of evaluated transcripts, with ablation experiments comparing repetition frequency and lexical diversity.

The study reports a clean-speech WER of 0.671 and an end-to-end RTF of 0.578. The selective-clarification mechanism has been evaluated offline; its impact on response correctness and hallucination remains subject to manual validation.
