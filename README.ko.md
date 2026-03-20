# Awesome NSFW AI 비디오 생성

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/ristponex/awesome-nsfw-ai-video/pulls)

무검열 AI 비디오 생성을 위한 모델, 도구, 프롬프트, 리소스의 엄선 목록입니다. 정기적으로 업데이트됩니다.

[English](README.md) | [简体中文](README.zh-CN.md) | [日本語](README.ja.md) | [한국어](#)

> **18세 이상 전용** — 이 리소스는 성인 전용입니다. 모든 콘텐츠는 관련 법률을 준수해야 합니다.

---

## 목차

- [모델](#모델)
  - [NSFW 최적화 모델](#nsfw-최적화-모델)
  - [NSFW 지원 범용 모델](#nsfw-지원-범용-모델)
  - [오픈 소스 / 셀프 호스팅](#오픈-소스--셀프-호스팅)
- [API 플랫폼](#api-플랫폼)
- [프롬프트 컬렉션](#프롬프트-컬렉션)
- [LoRA 리소스](#lora-리소스)
- [도구](#도구)
- [튜토리얼](#튜토리얼)
- [커뮤니티](#커뮤니티)
- [모델 비교](#모델-비교)
- [법률 및 윤리](#법률-및-윤리)
- [FAQ](#faq)

---

## 모델

### NSFW 최적화 모델

콘텐츠 필터 없이 성인 콘텐츠에 특화하여 파인튜닝된 모델입니다.

- ⭐ [Wan 2.2 Spicy I2V](https://www.atlascloud.ai/models/alibaba/wan-2.2-spicy/image-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - NSFW를 위해 LoRA 파인튜닝, 최고의 해부학적 정확도. **$0.03/초** | 480p–720p | 5–8초
- ⭐ [Wan 2.2 Spicy LoRA](https://www.atlascloud.ai/models/alibaba/wan-2.2-spicy/image-to-video-lora?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - NSFW 비디오를 위한 커스텀 LoRA 스타일. **$0.04/초** | 480p–720p | 5–8초 | 최대 6개 LoRA

### NSFW 지원 범용 모델

허용된 플랫폼을 통해 NSFW 콘텐츠를 지원하는 범용 비디오 모델입니다.

- [Wan 2.6 T2V](https://www.atlascloud.ai/models/alibaba/wan-2.6/text-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 텍스트-비디오, 멀티 카메라, 오디오 가이드. **$0.04–0.12/초** | 480p–1080p | 5–15초
- [Wan 2.6 I2V](https://www.atlascloud.ai/models/alibaba/wan-2.6/image-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 1080p 지원 이미지-비디오. **$0.10–0.15/초** | 720p–1080p | 5–15초
- [Wan 2.6 I2V Flash](https://www.atlascloud.ai/models/alibaba/wan-2.6/image-to-video-flash?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 저가형 I2V. **$0.018/초** | 720p–1080p | 5–15초
- [Wan 2.6 V2V](https://www.atlascloud.ai/models/alibaba/wan-2.6/video-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - characterX 표기를 사용한 비디오-비디오 변환. **$0.04–0.12/초** | 480p–1080p | 5–10초
- [Seedance v1.5 Pro T2V](https://www.atlascloud.ai/models/bytedance/seedance-v1.5-pro/text-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 네이티브 오디오-비주얼 동기화. **$0.222/비디오** | 480p–720p | 5초
- [Seedance v1.5 Pro I2V](https://www.atlascloud.ai/models/bytedance/seedance-v1.5-pro/image-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 시작+끝 프레임 이미지 애니메이션. **$0.222/비디오** | 480p–720p | 5초
- [Seedance v1.5 Fast](https://www.atlascloud.ai/models/bytedance/seedance-v1.5-pro/text-to-video-fast?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 오디오 포함 초저가 초안. **$0.018/비디오** | 720p | 5초
- [Vidu Q3-Pro T2V](https://www.atlascloud.ai/models/vidu/q3-pro/text-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 애니메이션 스타일 지원, BGM 생성. **$0.06–0.16/초** | 540p–1080p
- [Vidu Q3-Pro I2V](https://www.atlascloud.ai/models/vidu/q3-pro/image-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 애니메이션 모드 이미지 애니메이션. **$0.06–0.16/초** | 540p–1080p

### 오픈 소스 / 셀프 호스팅

자체 GPU에서 실행 — 완전한 제어, API 비용 없음.

- [Wan 2.1](https://github.com/Wan-Video/Wan2.1) - Apache 2.0, 커뮤니티 LoRA 사용 가능. Wan 2.2 Spicy의 기반.
- [CogVideoX](https://github.com/THUDM/CogVideo) - Zhipu AI의 오픈 소스. 480p–720p, 6초.
- [HunyuanVideo](https://github.com/Tencent/HunyuanVideo) - Tencent의 오픈 소스. 720p.
- [Mochi 1](https://github.com/genmoai/mochi) - Genmo의 오픈 소스. 스타일화된 출력.

---

## API 플랫폼

| 플랫폼 | NSFW 지원 | 비디오 모델 | 이미지 모델 | 가격 | 설정 |
|--------|:---------:|:----------:|:----------:|------|:----:|
| ⭐ [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) | 전체 | 100+ | 40+ | $0.03/초부터 | 쉬움 |
| [fal.ai](https://fal.ai) | 부분적 | 20+ | 30+ | $0.05/초부터 | 쉬움 |
| [Replicate](https://replicate.com) | 차단됨 | 50+ | 100+ | 다양 | 쉬움 |
| [RunPod](https://runpod.io) | 제한 없음 (셀프 호스팅) | 제한 없음 | 제한 없음 | GPU 렌탈 | 보통 |
| [ComfyUI](https://github.com/comfyanonymous/ComfyUI) | 제한 없음 (로컬) | 제한 없음 | 제한 없음 | 무료 + GPU | 어려움 |

---

## 프롬프트 컬렉션

- ⭐ [NSFW AI Video Prompts](https://github.com/ristponex/nsfw-ai-video-prompts) - 카테고리별로 정리된 100개 이상의 바로 사용 가능한 프롬프트
- ⭐ [Wan 2.2 Spicy Guide](https://github.com/ristponex/wan-spicy-nsfw-guide) - 완전한 API 예제가 포함된 50개 이상의 프롬프트
- [Wan 2.2 Spicy LoRA Guide](https://github.com/ristponex/wan-2.2-spicy-lora-nsfw) - LoRA 전용 프롬프트 및 스타일 가이드
- [NSFW AI Image Prompts](https://github.com/ristponex/nsfw-ai-image-prompts) - 이미지 생성 프롬프트 라이브러리

---

## LoRA 리소스

### NSFW LoRA를 찾을 수 있는 곳

- [Civitai](https://civitai.com) - 최대 LoRA 마켓플레이스. NSFW, 비디오 호환으로 필터링.
- [HuggingFace](https://huggingface.co/models?other=lora) - 오픈 소스 LoRA 모델
- [Tensor.Art](https://tensor.art) - 미리보기가 있는 커뮤니티 LoRA 갤러리
- [AIBooru](https://aibooru.online) - 연결된 LoRA가 있는 AI 아트 갤러리

### Wan 2.2 Spicy에서 LoRA 사용하기

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

## 도구

### 비디오 생성 인터페이스

- [ComfyUI](https://github.com/comfyanonymous/ComfyUI) - 로컬 생성을 위한 노드 기반 워크플로우
- [A1111 WebUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui) - 클래식 Stable Diffusion 인터페이스
- [Forge](https://github.com/lllyasviel/stable-diffusion-webui-forge) - 최적화된 A1111 포크

### 비디오 향상

- [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN) - 비디오/이미지 업스케일링
- [GFPGAN](https://github.com/TencentARC/GFPGAN) - 얼굴 복원
- [FFmpeg](https://ffmpeg.org) - 비디오 처리, 연결, 오디오 병합

### 오디오 동기화

- [FFmpeg Audio Merge](https://ffmpeg.org) - `ffmpeg -i video.mp4 -i audio.mp3 -c copy output.mp4`
- Wan 2.6 / Seedance v1.5 — 네이티브 `generate_audio` 파라미터

---

## 튜토리얼

### 시작하기

1. **[Wan 2.2 Spicy 완전 가이드](https://github.com/ristponex/wan-spicy-nsfw-guide)** — 제로에서 5분 만에 첫 번째 비디오 생성
2. **[LoRA 가이드](https://github.com/ristponex/ai-video-lora-guide)** — LoRA 어댑터를 사용한 커스텀 스타일
3. **[API 비교](https://github.com/ristponex/nsfw-ai-api-comparison)** — 적합한 플랫폼 찾기

### 프롬프트 엔지니어링

- 구체적인 해부학적 및 동작 설명 사용
- 조명 묘사: "soft studio lighting", "golden hour", "rim lighting"
- 카메라 방향: "close-up", "medium shot", "slow pan"
- 네거티브 프롬프트: "blurry, distorted, watermark, text"

### 참조 이미지 팁

- 고품질 소스 이미지 사용 (720p 이상 권장)
- 깨끗한 배경, 좋은 조명, 선명한 피사체
- 필요시 Flux Dev로 참조 이미지 생성

---

## 커뮤니티

### Reddit

- [r/AiNSFW](https://reddit.com/r/AiNSFW) - 일반 AI NSFW 토론
- [r/unstable_diffusion](https://reddit.com/r/unstable_diffusion) - 무검열 AI 아트
- [r/sdnsfw](https://reddit.com/r/sdnsfw) - Stable Diffusion NSFW
- [r/AIVideoGeneration](https://reddit.com/r/AIVideoGeneration) - AI 비디오 토론

### Discord

- [Civitai Discord](https://discord.gg/civitai) - 모델 공유 및 팁
- [ComfyUI Discord](https://discord.gg/comfyui) - 워크플로우 도움

---

## 모델 비교

| 기능 | Wan 2.2 Spicy | Wan 2.6 | Seedance 1.5 | Vidu Q3-Pro | 셀프 호스팅 |
|------|:------------:|:-------:|:------------:|:-----------:|:----------:|
| **NSFW 품질** | ★★★★★ | ★★★★☆ | ★★★★☆ | ★★★★☆ | ★★★★★ |
| **가격** | $0.03/초 | $0.04–0.15/초 | $0.018–0.222 | $0.06–0.16/초 | GPU 비용 |
| **최대 해상도** | 720p | 1080p | 720p | 1080p | 다양 |
| **최대 길이** | 8초 | 15초 | 5초 | 유연 | 다양 |
| **오디오** | ❌ | ✅ | ✅ | ✅ | 다양 |
| **LoRA** | ✅ | ❌ | ❌ | ❌ | ✅ |
| **애니메이션 스타일** | LoRA 통해 | ❌ | ❌ | ✅ 네이티브 | ✅ |
| **텍스트-비디오** | ❌ (I2V만) | ✅ | ✅ | ✅ | ✅ |
| **설정** | API 키 | API 키 | API 키 | API 키 | GPU + 설정 |

---

## 법률 및 윤리

### 허용되는 사용

- 개인 예술적 표현
- 라이선스를 받은 성인 엔터테인먼트 제작
- 학술/연구 목적
- 패션 및 파인 아트 사진

### 엄격히 금지

- 미성년자 관련 콘텐츠 (무관용)
- 실제 인물의 비동의 딥페이크
- 현지 법률을 위반하는 콘텐츠
- 괴롭힘 또는 보복 콘텐츠

### 모범 사례

- 모든 시청자 및 사용자의 연령 확인
- 가상의 캐릭터만 사용하거나 명시적 동의 획득
- AI 생성 콘텐츠를 명확히 표시
- 관할 지역의 법률 준수

---

## FAQ

<details>
<summary><b>NSFW 비디오를 생성하는 가장 저렴한 방법은 무엇인가요?</b></summary>
Atlas Cloud를 통한 Wan 2.2 Spicy, $0.03/초 — 5초 비디오가 단 $0.15입니다.
</details>

<details>
<summary><b>어떤 모델이 가장 좋은 NSFW 품질을 제공하나요?</b></summary>
Wan 2.2 Spicy (커스텀 스타일을 위한 LoRA 버전). 성인 콘텐츠를 위해 특별히 제작되어 해부학적 정확도와 동작이 파인튜닝되었습니다.
</details>

<details>
<summary><b>텍스트-비디오 NSFW 생성이 가능한가요?</b></summary>
Wan 2.2 Spicy는 이미지-비디오(I2V)만 지원합니다. 텍스트-비디오 NSFW의 경우 Wan 2.6 T2V 또는 Seedance v1.5를 사용하세요.
</details>

<details>
<summary><b>NSFW AI 비디오를 생성하는 것이 합법인가요?</b></summary>
대부분의 관할 지역에서 개인 용도로 가상 캐릭터의 NSFW 콘텐츠를 생성하는 것은 합법입니다. 항상 현지 법률을 확인하세요. 미성년자 관련 콘텐츠는 절대 생성하지 마세요.
</details>

<details>
<summary><b>강력한 컴퓨터가 필요한가요?</b></summary>
아니요 — API 기반 서비스는 클라우드 GPU에서 실행됩니다. 인터넷 연결과 API 키만 있으면 됩니다.
</details>

<details>
<summary><b>더 좋은 결과를 얻으려면 어떻게 해야 하나요?</b></summary>
고품질 참조 이미지를 사용하고, 상세한 프롬프트를 작성하고, LoRA 스타일을 실험해 보세요. 위의 프롬프트 컬렉션을 참조하세요.
</details>

---

## 기여하기

새로운 모델을 발견하셨나요? 유용한 리소스가 있나요? PR을 보내주세요!

- `- [이름](URL) - 설명` 형식을 따르세요
- 가격 및 주요 사양을 포함하세요
- 제출 전에 리소스를 테스트하세요
- 설명은 간결하고 사실적으로 작성하세요

---

## 라이선스

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

법률이 허용하는 범위 내에서 기여자들은 이 작업에 대한 모든 저작권 및 관련 권리를 포기했습니다.
