# Awesome-AI-Audio-Enhancement

# Top AI Audio Enhancement Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Speech Enhancement, Noise Reduction & Studio-Quality Audio Restoration*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **AI Audio Enhancement**. These tools enable podcasters, video creators, and enterprises to transform noisy, echoey, or low-quality recordings into clean, broadcast-ready audio using AI-powered noise reduction, voice isolation, and studio sound reconstruction.

**Examples** include Adobe Podcast, ElevenLabs, Descript Studio Sound, Auphonic, Krisp, Cleanvoice AI, Lalal.ai, Podcastle, Dolby.io, and Resemble AI (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom speech enhancement models, and open audio processing pipelines—ideal for developers, researchers, and organizations seeking transparent, vendor-independent audio enhancement.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Adobe Podcast](https://podcast.adobe.com/enhance)**  
  Web-based AI audio enhancement tool with free Enhance Speech feature. Language-agnostic voice isolation that filters noise, adjusts pitch and volume, and normalizes audio. Works best on clear speech inputs—not designed for music or sound effects. No account required for basic use .

- **[ElevenLabs Studio](https://elevenlabs.io/studio)**  
  Agentic AI editor with Voice Isolator for removing background noise, reverb, and distracting sounds. Features expressive AI voiceovers, music generation, sound effects, captions, and video editing. Supports 30+ languages with API access .

- **[Descript Studio Sound](https://help.descript.com/effects-animations-transitions/studio-sound)**  
  AI-powered audio effect that reduces background noise, echo, and room reverb for spoken voice. Applied at file level with adjustable Intensity slider. Requires internet connection. Works on recorded audio, not AI-generated speech .

- **[Auphonic](https://auphonic.com/)**  
  Automated audio post-production with Studio Voice (beta) for reconstructing studio-quality voice from noisy recordings. Features Adaptive Leveler with editable gain curve, Denoising Segment Editor for precise noise reduction control, Mic Bleed Remover for multitrack sessions, and Automatic Cutting for removing silence, filler words, and music segments .

- **[Krisp](https://krisp.ai/)**  
  Real-time noise cancellation and voice isolation for calls and recordings. Voice Isolation 2.5 reduces STT word error rate by 46.4% on average, with 69.7% fewer errors on competing speech. Customer Accent Conversion softens accents in real-time for improved agent comprehension in call centers .

- **[Cleanvoice AI](https://cleanvoice.ai/)**  
  AI audio cleaning with filler word removal ("um", "uh", "like"), long silence trimming, mouth sound removal, breath removal, and stutter removal. Features studio sound enhancement, noise reduction, normalization, and multi-track merging. Configurable via REST API .

- **[Lalal.ai](https://www.lalal.ai/)**  
  AI stem separation and audio enhancement. Features echo and reverb remover for vocals, noise reduction, and voice isolation. Used at scale by LifeOnRecord processing 100,000+ minutes annually. Supports API access for automated workflows .

- **[Podcastle](https://podcastle.ai/)**  
  AI-powered audio and video recording/editing platform. Magic Dust feature provides one-click noise reduction, EQ, and vocal enhancement. Also offers AI voiceovers, transcription, and video editing .

- **[Dolby.io](https://dolby.io/)**  
  Media processing APIs for audio enhancement. Features loudness normalization, noise reduction, dynamic range control, and EQ. Used in podcast post-production pipelines via CLI tools .

- **[Resemble AI](https://www.resemble.ai/)**  
  Voice cloning and speech synthesis with enhance models. Resemble Enhance provides denoising and speech enhancement via 2D UNet spectral-mask denoiser and conditional flow matching .

## Open-Source GitHub Projects

- **[Resemble Enhance (MLX)](https://huggingface.co/smcleod/resemble-enhance-mlx)**  
  MLX-compatible weights for Resemble AI's enhance model (CC-BY-NC-4.0, non-commercial). Converts PyTorch checkpoint to Apple Silicon MLX format. Features denoiser (41 MB), IRMAE encoder/decoder (390 MB), conditional flow matching (264 MB), and UnivNet vocoder (662 MB). Run via `resemble-enhance-swift` on macOS .

- **[audio-super-resolution](https://pypi.org/project/audio-super-resolution/)**  
  Python CLI and library for audio super-resolution and bandwidth extension. Features deterministic sinc-resample baseline, optional AudioSR backend, LavaSR-compatible managed weight metadata, JSON run manifests, and quality reports. Supports batch processing and regression workflows .

- **[UniVoiceLite](https://github.com/jisoo-o/UniVoiceLite)**  
  Lightweight unsupervised audio-visual framework unifying speech enhancement and separation (IEEE Xplore, Dec 2025). Leverages lip motion and facial identity cues with Wasserstein distance regularization. Achieves strong performance in noisy and multi-speaker scenarios without paired noisy-clean data .

- **[Teaching Python Post-Production CLI](https://github.com/teachingpython/post-production)**  
  Command-line pipeline for podcast post-production (open-source). Features Dolby.io audio enhancement (loudness, noise reduction, dynamic range, EQ), AssemblyAI transcription, filler-word removal, and transcoding. Replaces manual multi-step workflows with single tool .

### Additional Strong Open-Source Options

- **[DeepFilterNet](https://github.com/Rikorose/DeepFilterNet)** — Real-time speech enhancement for full-band audio (MIT). Deep filtering for noise suppression on embedded devices.
- **[RNNoise](https://github.com/xiph/rnnoise)** — Recurrent neural network for noise suppression (BSD-3-Clause). Lightweight, runs in real-time on CPU.
- **[Demucs](https://github.com/facebookresearch/demucs)** — Music source separation (MIT) from Meta. Separates vocals, drums, bass, and other instruments.
- **[Spleeter](https://github.com/deezer/spleeter)** — Deezer's source separation library (MIT). Fast stem separation for audio enhancement.
- Community **n8n** workflows for automated audio enhancement pipelines and batch processing.

**Frameworks for building custom systems**: Combine **Resemble Enhance (MLX)** or **DeepFilterNet** as the speech enhancement engine with **audio-super-resolution** for bandwidth extension, **Demucs** or **Spleeter** for source separation, **RNNoise** for lightweight real-time denoising, and **Python/FastAPI** for pipeline orchestration—creating a fully self-hosted, enterprise-grade AI audio enhancement platform.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- AI audio enhancement tools processing voice recordings must comply with data protection regulations (GDPR, CCPA, etc.) and consent requirements for voice cloning.
- Self-hosted open-source solutions require proper GPU provisioning for neural models, audio quality validation, and ongoing maintenance. Voice enhancement works best on clear speech inputs—music, sound effects, and layered non-speech audio may produce unnatural results . Non-commercial licenses (CC-BY-NC) restrict commercial deployment of some open-source models.

---

**Made for podcasters, video creators, audio engineers, and developers building transparent audio enhancement solutions.**  
Let's make AI Audio Enhancement more open, data-driven, and studio-quality.
