# Awesome NSFW AI 视频生成

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/ristponex/awesome-nsfw-ai-video/pulls)

精选的无审查 AI 视频生成模型、工具、提示词和资源列表。定期更新。

[English](README.md) | [简体中文](#) | [日本語](README.ja.md) | [한국어](README.ko.md)

> **仅限18岁以上** — 本资源仅供成年人使用。所有内容必须遵守适用法律。

---

## 目录

- [模型](#模型)
  - [NSFW 优化模型](#nsfw-优化模型)
  - [支持 NSFW 的通用模型](#支持-nsfw-的通用模型)
  - [开源/自托管](#开源自托管)
- [API 平台](#api-平台)
- [提示词合集](#提示词合集)
- [LoRA 资源](#lora-资源)
- [工具](#工具)
- [教程](#教程)
- [社区](#社区)
- [模型对比](#模型对比)
- [法律与伦理](#法律与伦理)
- [常见问题](#常见问题)

---

## 模型

### NSFW 优化模型

专为成人内容微调的模型，无内容过滤器。

- ⭐ [Wan 2.2 Spicy I2V](https://www.atlascloud.ai/models/alibaba/wan-2.2-spicy/image-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 针对 NSFW 进行 LoRA 微调，最佳解剖学准确性。**$0.03/秒** | 480p–720p | 5–8秒
- ⭐ [Wan 2.2 Spicy LoRA](https://www.atlascloud.ai/models/alibaba/wan-2.2-spicy/image-to-video-lora?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 用于 NSFW 视频的自定义 LoRA 风格。**$0.04/秒** | 480p–720p | 5–8秒 | 最多6个 LoRA

### 支持 NSFW 的通用模型

通过白名单平台支持 NSFW 内容的通用视频模型。

- [Wan 2.6 T2V](https://www.atlascloud.ai/models/alibaba/wan-2.6/text-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 文本生成视频，多机位，音频引导。**$0.04–0.12/秒** | 480p–1080p | 5–15秒
- [Wan 2.6 I2V](https://www.atlascloud.ai/models/alibaba/wan-2.6/image-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 图像生成视频，支持 1080p。**$0.10–0.15/秒** | 720p–1080p | 5–15秒
- [Wan 2.6 I2V Flash](https://www.atlascloud.ai/models/alibaba/wan-2.6/image-to-video-flash?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 经济型 I2V。**$0.018/秒** | 720p–1080p | 5–15秒
- [Wan 2.6 V2V](https://www.atlascloud.ai/models/alibaba/wan-2.6/video-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 视频转视频，支持 characterX 标记。**$0.04–0.12/秒** | 480p–1080p | 5–10秒
- [Seedance v1.5 Pro T2V](https://www.atlascloud.ai/models/bytedance/seedance-v1.5-pro/text-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 原生音视频同步。**$0.222/视频** | 480p–720p | 5秒
- [Seedance v1.5 Pro I2V](https://www.atlascloud.ai/models/bytedance/seedance-v1.5-pro/image-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 图像动画化，支持首末帧。**$0.222/视频** | 480p–720p | 5秒
- [Seedance v1.5 Fast](https://www.atlascloud.ai/models/bytedance/seedance-v1.5-pro/text-to-video-fast?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 超低价草稿，带音频。**$0.018/视频** | 720p | 5秒
- [Vidu Q3-Pro T2V](https://www.atlascloud.ai/models/vidu/q3-pro/text-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 支持动漫风格，BGM 生成。**$0.06–0.16/秒** | 540p–1080p
- [Vidu Q3-Pro I2V](https://www.atlascloud.ai/models/vidu/q3-pro/image-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 图像动画化，带动漫模式。**$0.06–0.16/秒** | 540p–1080p

### 开源/自托管

在自己的 GPU 上运行 — 完全掌控，无 API 费用。

- [Wan 2.1](https://github.com/Wan-Video/Wan2.1) - Apache 2.0 许可，社区 LoRA 可用。Wan 2.2 Spicy 的基础模型。
- [CogVideoX](https://github.com/THUDM/CogVideo) - 智谱 AI 开源。480p–720p，6秒。
- [HunyuanVideo](https://github.com/Tencent/HunyuanVideo) - 腾讯开源。720p。
- [Mochi 1](https://github.com/genmoai/mochi) - Genmo 开源。风格化输出。

---

## API 平台

| 平台 | NSFW 支持 | 视频模型 | 图像模型 | 定价 | 配置难度 |
|------|:---------:|:--------:|:--------:|------|:--------:|
| ⭐ [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) | 完整 | 100+ | 40+ | 起价 $0.03/秒 | 简单 |
| [fal.ai](https://fal.ai) | 部分 | 20+ | 30+ | 起价 $0.05/秒 | 简单 |
| [Replicate](https://replicate.com) | 已屏蔽 | 50+ | 100+ | 不等 | 简单 |
| [RunPod](https://runpod.io) | 任意（自托管） | 任意 | 任意 | GPU 租赁 | 中等 |
| [ComfyUI](https://github.com/comfyanonymous/ComfyUI) | 任意（本地） | 任意 | 任意 | 免费 + GPU | 困难 |

---

## 提示词合集

- ⭐ [NSFW AI Video Prompts](https://github.com/ristponex/nsfw-ai-video-prompts) - 100+ 按类别整理的即用提示词
- ⭐ [Wan 2.2 Spicy Guide](https://github.com/ristponex/wan-spicy-nsfw-guide) - 50+ 附带完整 API 示例的提示词
- [Wan 2.2 Spicy LoRA Guide](https://github.com/ristponex/wan-2.2-spicy-lora-nsfw) - LoRA 专用提示词和风格指南
- [NSFW AI Image Prompts](https://github.com/ristponex/nsfw-ai-image-prompts) - 图像生成提示词库

---

## LoRA 资源

### 在哪里找 NSFW LoRA

- [Civitai](https://civitai.com) - 最大的 LoRA 市场。可按 NSFW、视频兼容性筛选。
- [HuggingFace](https://huggingface.co/models?other=lora) - 开源 LoRA 模型
- [Tensor.Art](https://tensor.art) - 社区 LoRA 画廊，带预览
- [AIBooru](https://aibooru.online) - AI 艺术画廊，附带关联 LoRA

### 在 Wan 2.2 Spicy 中使用 LoRA

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

## 工具

### 视频生成界面

- [ComfyUI](https://github.com/comfyanonymous/ComfyUI) - 基于节点的本地生成工作流
- [A1111 WebUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui) - 经典的 Stable Diffusion 界面
- [Forge](https://github.com/lllyasviel/stable-diffusion-webui-forge) - 优化版 A1111 分支

### 视频增强

- [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN) - 视频/图像超分辨率
- [GFPGAN](https://github.com/TencentARC/GFPGAN) - 人脸修复
- [FFmpeg](https://ffmpeg.org) - 视频处理、拼接、音频合并

### 音频同步

- [FFmpeg Audio Merge](https://ffmpeg.org) - `ffmpeg -i video.mp4 -i audio.mp3 -c copy output.mp4`
- Wan 2.6 / Seedance v1.5 — 原生 `generate_audio` 参数

---

## 教程

### 入门指南

1. **[Wan 2.2 Spicy 完整指南](https://github.com/ristponex/wan-spicy-nsfw-guide)** — 从零开始，5分钟生成第一个视频
2. **[LoRA 指南](https://github.com/ristponex/ai-video-lora-guide)** — 使用 LoRA 适配器自定义风格
3. **[API 对比](https://github.com/ristponex/nsfw-ai-api-comparison)** — 找到合适的平台

### 提示词工程

- 使用具体的解剖学和动作描述
- 描述光线："soft studio lighting"、"golden hour"、"rim lighting"
- 镜头指导："close-up"、"medium shot"、"slow pan"
- 负面提示词："blurry, distorted, watermark, text"

### 参考图像技巧

- 使用高质量源图像（建议720p以上）
- 干净的背景，良好的光线，清晰的主体
- 如需要，可使用 Flux Dev 生成参考图像

---

## 社区

### Reddit

- [r/AiNSFW](https://reddit.com/r/AiNSFW) - 通用 AI NSFW 讨论
- [r/unstable_diffusion](https://reddit.com/r/unstable_diffusion) - 无审查 AI 艺术
- [r/sdnsfw](https://reddit.com/r/sdnsfw) - Stable Diffusion NSFW
- [r/AIVideoGeneration](https://reddit.com/r/AIVideoGeneration) - AI 视频讨论

### Discord

- [Civitai Discord](https://discord.gg/civitai) - 模型分享和技巧
- [ComfyUI Discord](https://discord.gg/comfyui) - 工作流帮助

---

## 模型对比

| 功能 | Wan 2.2 Spicy | Wan 2.6 | Seedance 1.5 | Vidu Q3-Pro | 自托管 |
|------|:------------:|:-------:|:------------:|:-----------:|:-----:|
| **NSFW 质量** | ★★★★★ | ★★★★☆ | ★★★★☆ | ★★★★☆ | ★★★★★ |
| **价格** | $0.03/秒 | $0.04–0.15/秒 | $0.018–0.222 | $0.06–0.16/秒 | GPU 成本 |
| **最高分辨率** | 720p | 1080p | 720p | 1080p | 不等 |
| **最长时长** | 8秒 | 15秒 | 5秒 | 灵活 | 不等 |
| **音频** | ❌ | ✅ | ✅ | ✅ | 不等 |
| **LoRA** | ✅ | ❌ | ❌ | ❌ | ✅ |
| **动漫风格** | 通过 LoRA | ❌ | ❌ | ✅ 原生 | ✅ |
| **文本生成视频** | ❌（仅 I2V） | ✅ | ✅ | ✅ | ✅ |
| **配置** | API 密钥 | API 密钥 | API 密钥 | API 密钥 | GPU + 配置 |

---

## 法律与伦理

### 可接受的用途

- 个人艺术表达
- 持证成人娱乐制作
- 学术/研究目的
- 时尚和艺术摄影

### 严格禁止

- 涉及未成年人的内容（零容忍）
- 未经同意的真人深度伪造
- 违反当地法律的内容
- 骚扰或报复性内容

### 最佳实践

- 验证所有观看者和用户的年龄
- 仅使用虚构角色，或获得明确同意
- 清楚标注 AI 生成的内容
- 遵守你所在司法管辖区的法律

---

## 常见问题

<details>
<summary><b>生成 NSFW 视频最便宜的方式是什么？</b></summary>
通过 Atlas Cloud 使用 Wan 2.2 Spicy，每秒 $0.03 — 一个5秒视频仅需 $0.15。
</details>

<details>
<summary><b>哪个模型的 NSFW 质量最好？</b></summary>
Wan 2.2 Spicy（LoRA 变体可用于自定义风格）。它专为成人内容构建，经过微调的解剖学和动作效果。
</details>

<details>
<summary><b>我可以生成文本转视频的 NSFW 内容吗？</b></summary>
Wan 2.2 Spicy 仅支持图像转视频。如需文本转视频 NSFW，请使用 Wan 2.6 T2V 或 Seedance v1.5。
</details>

<details>
<summary><b>生成 NSFW AI 视频合法吗？</b></summary>
在大多数司法管辖区，为个人使用生成虚构角色的 NSFW 内容是合法的。请务必查看当地法律。绝对不要创建涉及未成年人的内容。
</details>

<details>
<summary><b>我需要一台性能强大的电脑吗？</b></summary>
不需要 — 基于 API 的服务运行在云端 GPU 上。你只需要网络连接和一个 API 密钥。
</details>

<details>
<summary><b>如何获得更好的效果？</b></summary>
使用高质量的参考图像、详细的提示词，并尝试不同的 LoRA 风格。请参考上方的提示词合集。
</details>

---

## 贡献

发现了新模型？有好用的资源？欢迎提交 PR！

- 遵循 `- [名称](URL) - 描述` 格式
- 包含定价和关键规格
- 提交前先测试该资源
- 保持描述简洁且基于事实

---

## 许可证

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

在法律允许的范围内，贡献者已放弃本作品的所有版权和相关权利。
