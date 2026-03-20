# Awesome NSFW AI Video Generation

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/ristponex/awesome-nsfw-ai-video/pulls)

A curated list of models, tools, prompts, and resources for uncensored AI video generation. Updated regularly.

[English](#) | [简体中文](README.zh-CN.md) | [日本語](README.ja.md) | [한국어](README.ko.md)

> **18+ Only** — This resource is for adults. All content must comply with applicable laws.

---

## Contents

- [Models](#models)
  - [NSFW-Optimized Models](#nsfw-optimized-models)
  - [General Models with NSFW Support](#general-models-with-nsfw-support)
  - [Open Source / Self-Hosted](#open-source--self-hosted)
- [API Platforms](#api-platforms)
- [Prompt Collections](#prompt-collections)
- [LoRA Resources](#lora-resources)
- [Tools](#tools)
- [Tutorials](#tutorials)
- [Community](#community)
- [Model Comparison](#model-comparison)
- [Legal & Ethics](#legal--ethics)
- [FAQ](#faq)

---

## Models

### NSFW-Optimized Models

Models specifically fine-tuned for mature content with no content filters.

- ⭐ [Wan 2.2 Spicy I2V](https://www.atlascloud.ai/models/alibaba/wan-2.2-spicy/image-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - LoRA fine-tuned for NSFW, best anatomical accuracy. **$0.03/s** | 480p–720p | 5–8s
- ⭐ [Wan 2.2 Spicy LoRA](https://www.atlascloud.ai/models/alibaba/wan-2.2-spicy/image-to-video-lora?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - Custom LoRA styles for NSFW video. **$0.04/s** | 480p–720p | 5–8s | Up to 6 LoRAs

### General Models with NSFW Support

General-purpose video models that support NSFW content via whitelisted platforms.

- [Wan 2.6 T2V](https://www.atlascloud.ai/models/alibaba/wan-2.6/text-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - Text-to-video, multi-camera, audio-guided. **$0.04–0.12/s** | 480p–1080p | 5–15s
- [Wan 2.6 I2V](https://www.atlascloud.ai/models/alibaba/wan-2.6/image-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - Image-to-video with 1080p support. **$0.10–0.15/s** | 720p–1080p | 5–15s
- [Wan 2.6 I2V Flash](https://www.atlascloud.ai/models/alibaba/wan-2.6/image-to-video-flash?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - Budget I2V. **$0.018/s** | 720p–1080p | 5–15s
- [Wan 2.6 V2V](https://www.atlascloud.ai/models/alibaba/wan-2.6/video-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - Video-to-video transfer with characterX notation. **$0.04–0.12/s** | 480p–1080p | 5–10s
- [Seedance v1.5 Pro T2V](https://www.atlascloud.ai/models/bytedance/seedance-v1.5-pro/text-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - Native audio-visual sync. **$0.222/video** | 480p–720p | 5s
- [Seedance v1.5 Pro I2V](https://www.atlascloud.ai/models/bytedance/seedance-v1.5-pro/image-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - Image animation with start+end frames. **$0.222/video** | 480p–720p | 5s
- [Seedance v1.5 Fast](https://www.atlascloud.ai/models/bytedance/seedance-v1.5-pro/text-to-video-fast?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - Ultra-cheap drafts with audio. **$0.018/video** | 720p | 5s
- [Vidu Q3-Pro T2V](https://www.atlascloud.ai/models/vidu/q3-pro/text-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - Anime style support, BGM generation. **$0.06–0.16/s** | 540p–1080p
- [Vidu Q3-Pro I2V](https://www.atlascloud.ai/models/vidu/q3-pro/image-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - Image animation with anime mode. **$0.06–0.16/s** | 540p–1080p

### Open Source / Self-Hosted

Run on your own GPU — full control, no API costs.

- [Wan 2.1](https://github.com/Wan-Video/Wan2.1) - Apache 2.0, community LoRAs available. Basis for Wan 2.2 Spicy.
- [CogVideoX](https://github.com/THUDM/CogVideo) - Open-source by Zhipu AI. 480p–720p, 6s.
- [HunyuanVideo](https://github.com/Tencent/HunyuanVideo) - Open-source by Tencent. 720p.
- [Mochi 1](https://github.com/genmoai/mochi) - Open-source by Genmo. Stylized output.

---

## API Platforms

| Platform | NSFW Support | Video Models | Image Models | Pricing | Setup |
|----------|:------------:|:------------:|:------------:|---------|:-----:|
| ⭐ [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) | Full | 100+ | 40+ | From $0.03/s | Easy |
| [fal.ai](https://fal.ai) | Partial | 20+ | 30+ | From $0.05/s | Easy |
| [Replicate](https://replicate.com) | Blocked | 50+ | 100+ | Varies | Easy |
| [RunPod](https://runpod.io) | Any (self-host) | Any | Any | GPU rental | Medium |
| [ComfyUI](https://github.com/comfyanonymous/ComfyUI) | Any (local) | Any | Any | Free + GPU | Hard |

---

## Prompt Collections

- ⭐ [NSFW AI Video Prompts](https://github.com/ristponex/nsfw-ai-video-prompts) - 100+ copy-paste ready prompts organized by category
- ⭐ [Wan 2.2 Spicy Guide](https://github.com/ristponex/wan-spicy-nsfw-guide) - 50+ prompts with complete API examples
- [Wan 2.2 Spicy LoRA Guide](https://github.com/ristponex/wan-2.2-spicy-lora-nsfw) - LoRA-specific prompts and style guide
- [NSFW AI Image Prompts](https://github.com/ristponex/nsfw-ai-image-prompts) - Image generation prompt library

---

## LoRA Resources

### Where to Find NSFW LoRAs

- [Civitai](https://civitai.com) - Largest LoRA marketplace. Filter by NSFW, video-compatible.
- [HuggingFace](https://huggingface.co/models?other=lora) - Open-source LoRA models
- [Tensor.Art](https://tensor.art) - Community LoRA gallery with previews
- [AIBooru](https://aibooru.online) - AI art gallery with linked LoRAs

### Using LoRAs with Wan 2.2 Spicy

```bash
curl -s -X POST "https://api.atlascloud.ai/api/v1/model/generateVideo" \
  -H "Authorization: Bearer $ATLASCLOUD_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "alibaba/wan-2.2-spicy/image-to-video-lora",
    "image": "https://example.com/reference.jpg",
    "prompt": "Elegant movement, soft lighting",
    "resolution": "720p",
    "duration": 5,
    "high_noise_loras": ["https://civitai.com/api/download/models/12345"],
    "low_noise_loras": ["https://civitai.com/api/download/models/67890"]
  }'
```

---

## Tools

### Video Generation Interfaces

- [ComfyUI](https://github.com/comfyanonymous/ComfyUI) - Node-based workflow for local generation
- [A1111 WebUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui) - Classic Stable Diffusion interface
- [Forge](https://github.com/lllyasviel/stable-diffusion-webui-forge) - Optimized A1111 fork

### Video Enhancement

- [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN) - Video/image upscaling
- [GFPGAN](https://github.com/TencentARC/GFPGAN) - Face restoration
- [FFmpeg](https://ffmpeg.org) - Video processing, concatenation, audio merge

### Audio Sync

- [FFmpeg Audio Merge](https://ffmpeg.org) - `ffmpeg -i video.mp4 -i audio.mp3 -c copy output.mp4`
- Wan 2.6 / Seedance v1.5 — native `generate_audio` parameter

---

## Tutorials

### Getting Started

1. **[Wan 2.2 Spicy Complete Guide](https://github.com/ristponex/wan-spicy-nsfw-guide)** — From zero to first video in 5 minutes
2. **[LoRA Guide](https://github.com/ristponex/ai-video-lora-guide)** — Custom styles with LoRA adapters
3. **[API Comparison](https://github.com/ristponex/nsfw-ai-api-comparison)** — Find the right platform

### Prompt Engineering

- Use specific anatomical and movement descriptions
- Describe lighting: "soft studio lighting", "golden hour", "rim lighting"
- Camera direction: "close-up", "medium shot", "slow pan"
- Negative prompts: "blurry, distorted, watermark, text"

### Reference Image Tips

- Use high-quality source images (720p+ recommended)
- Clean background, good lighting, clear subject
- Generate reference images with Flux Dev if needed

---

## Community

### Reddit

- [r/AiNSFW](https://reddit.com/r/AiNSFW) - General AI NSFW discussion
- [r/unstable_diffusion](https://reddit.com/r/unstable_diffusion) - Uncensored AI art
- [r/sdnsfw](https://reddit.com/r/sdnsfw) - Stable Diffusion NSFW
- [r/AIVideoGeneration](https://reddit.com/r/AIVideoGeneration) - AI video discussion

### Discord

- [Civitai Discord](https://discord.gg/civitai) - Model sharing and tips
- [ComfyUI Discord](https://discord.gg/comfyui) - Workflow help

---

## Model Comparison

| Feature | Wan 2.2 Spicy | Wan 2.6 | Seedance 1.5 | Vidu Q3-Pro | Self-Hosted |
|---------|:------------:|:-------:|:------------:|:-----------:|:-----------:|
| **NSFW Quality** | ★★★★★ | ★★★★☆ | ★★★★☆ | ★★★★☆ | ★★★★★ |
| **Price** | $0.03/s | $0.04–0.15/s | $0.018–0.222 | $0.06–0.16/s | GPU cost |
| **Max Resolution** | 720p | 1080p | 720p | 1080p | Varies |
| **Max Duration** | 8s | 15s | 5s | Flexible | Varies |
| **Audio** | ❌ | ✅ | ✅ | ✅ | Varies |
| **LoRA** | ✅ | ❌ | ❌ | ❌ | ✅ |
| **Anime Style** | Via LoRA | ❌ | ❌ | ✅ Native | ✅ |
| **Text-to-Video** | ❌ (I2V only) | ✅ | ✅ | ✅ | ✅ |
| **Setup** | API key | API key | API key | API key | GPU + setup |

---

## Legal & Ethics

### Acceptable Use

- Personal artistic expression
- Licensed adult entertainment production
- Academic/research purposes
- Fashion and fine art photography

### Strictly Prohibited

- Content involving minors (zero tolerance)
- Non-consensual deepfakes of real people
- Content violating local laws
- Harassment or revenge content

### Best Practices

- Verify age of all viewers and users
- Use fictional characters only, or obtain explicit consent
- Label AI-generated content clearly
- Comply with your jurisdiction's laws

---

## FAQ

<details>
<summary><b>What's the cheapest way to generate NSFW videos?</b></summary>
Wan 2.2 Spicy at $0.03/s via Atlas Cloud — a 5-second video costs just $0.15.
</details>

<details>
<summary><b>Which model has the best NSFW quality?</b></summary>
Wan 2.2 Spicy (LoRA variant for custom styles). It's purpose-built for mature content with fine-tuned anatomy and motion.
</details>

<details>
<summary><b>Can I generate text-to-video NSFW?</b></summary>
Wan 2.2 Spicy is image-to-video only. For text-to-video NSFW, use Wan 2.6 T2V or Seedance v1.5.
</details>

<details>
<summary><b>Is it legal to generate NSFW AI videos?</b></summary>
In most jurisdictions, generating NSFW content of fictional characters for personal use is legal. Always check your local laws. Never create content involving minors.
</details>

<details>
<summary><b>Do I need a powerful computer?</b></summary>
No — API-based services run on cloud GPUs. You just need an internet connection and an API key.
</details>

<details>
<summary><b>How do I get better results?</b></summary>
Use high-quality reference images, detailed prompts, and experiment with LoRA styles. See our prompt collections above.
</details>

---

## Contributing

Found a new model? Have a useful resource? Open a PR!

- Follow the `- [Name](URL) - Description` format
- Include pricing and key specs
- Test the resource before submitting
- Keep descriptions concise and factual

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related rights to this work.
