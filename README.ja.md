# Awesome NSFW AI動画生成

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/ristponex/awesome-nsfw-ai-video/pulls)

無検閲AI動画生成のためのモデル、ツール、プロンプト、リソースの厳選リストです。定期的に更新されます。

[English](README.md) | [简体中文](README.zh-CN.md) | [日本語](#) | [한국어](README.ko.md)

> **18歳以上限定** — このリソースは成人向けです。すべてのコンテンツは適用される法律に準拠する必要があります。

---

## 目次

- [モデル](#モデル)
  - [NSFW最適化モデル](#nsfw最適化モデル)
  - [NSFWサポート付き汎用モデル](#nsfwサポート付き汎用モデル)
  - [オープンソース / セルフホスト](#オープンソース--セルフホスト)
- [APIプラットフォーム](#apiプラットフォーム)
- [プロンプトコレクション](#プロンプトコレクション)
- [LoRAリソース](#loraリソース)
- [ツール](#ツール)
- [チュートリアル](#チュートリアル)
- [コミュニティ](#コミュニティ)
- [モデル比較](#モデル比較)
- [法律と倫理](#法律と倫理)
- [FAQ](#faq)

---

## モデル

### NSFW最適化モデル

コンテンツフィルターなしで、成人向けコンテンツ用に特別にファインチューニングされたモデルです。

- ⭐ [Wan 2.2 Spicy I2V](https://www.atlascloud.ai/models/alibaba/wan-2.2-spicy/image-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - NSFW用にLoRAファインチューニング、最高の解剖学的精度。**$0.03/秒** | 480p–720p | 5–8秒
- ⭐ [Wan 2.2 Spicy LoRA](https://www.atlascloud.ai/models/alibaba/wan-2.2-spicy/image-to-video-lora?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - NSFW動画用カスタムLoRAスタイル。**$0.04/秒** | 480p–720p | 5–8秒 | 最大6つのLoRA

### NSFWサポート付き汎用モデル

ホワイトリストされたプラットフォーム経由でNSFWコンテンツをサポートする汎用動画モデルです。

- [Wan 2.6 T2V](https://www.atlascloud.ai/models/alibaba/wan-2.6/text-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - テキストから動画、マルチカメラ、音声ガイド対応。**$0.04–0.12/秒** | 480p–1080p | 5–15秒
- [Wan 2.6 I2V](https://www.atlascloud.ai/models/alibaba/wan-2.6/image-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 画像から動画、1080pサポート。**$0.10–0.15/秒** | 720p–1080p | 5–15秒
- [Wan 2.6 I2V Flash](https://www.atlascloud.ai/models/alibaba/wan-2.6/image-to-video-flash?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 低価格I2V。**$0.018/秒** | 720p–1080p | 5–15秒
- [Wan 2.6 V2V](https://www.atlascloud.ai/models/alibaba/wan-2.6/video-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - characterX記法による動画間変換。**$0.04–0.12/秒** | 480p–1080p | 5–10秒
- [Seedance v1.5 Pro T2V](https://www.atlascloud.ai/models/bytedance/seedance-v1.5-pro/text-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - ネイティブ音声映像同期。**$0.222/動画** | 480p–720p | 5秒
- [Seedance v1.5 Pro I2V](https://www.atlascloud.ai/models/bytedance/seedance-v1.5-pro/image-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 開始+終了フレームによる画像アニメーション。**$0.222/動画** | 480p–720p | 5秒
- [Seedance v1.5 Fast](https://www.atlascloud.ai/models/bytedance/seedance-v1.5-pro/text-to-video-fast?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - 音声付き超低価格ドラフト。**$0.018/動画** | 720p | 5秒
- [Vidu Q3-Pro T2V](https://www.atlascloud.ai/models/vidu/q3-pro/text-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - アニメスタイルサポート、BGM生成。**$0.06–0.16/秒** | 540p–1080p
- [Vidu Q3-Pro I2V](https://www.atlascloud.ai/models/vidu/q3-pro/image-to-video?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) - アニメモード付き画像アニメーション。**$0.06–0.16/秒** | 540p–1080p

### オープンソース / セルフホスト

自前のGPUで実行 — 完全制御、API費用なし。

- [Wan 2.1](https://github.com/Wan-Video/Wan2.1) - Apache 2.0、コミュニティLoRA利用可能。Wan 2.2 Spicyのベース。
- [CogVideoX](https://github.com/THUDM/CogVideo) - Zhipu AIによるオープンソース。480p–720p、6秒。
- [HunyuanVideo](https://github.com/Tencent/HunyuanVideo) - Tencentによるオープンソース。720p。
- [Mochi 1](https://github.com/genmoai/mochi) - Genmoによるオープンソース。スタイライズド出力。

---

## APIプラットフォーム

| プラットフォーム | NSFWサポート | 動画モデル | 画像モデル | 価格 | セットアップ |
|----------|:------------:|:------------:|:------------:|---------|:-----:|
| ⭐ [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=awesome-nsfw-ai-video) | フル | 100+ | 40+ | $0.03/秒〜 | 簡単 |
| [fal.ai](https://fal.ai) | 部分的 | 20+ | 30+ | $0.05/秒〜 | 簡単 |
| [Replicate](https://replicate.com) | ブロック | 50+ | 100+ | 変動制 | 簡単 |
| [RunPod](https://runpod.io) | 任意（セルフホスト） | 任意 | 任意 | GPUレンタル | 中程度 |
| [ComfyUI](https://github.com/comfyanonymous/ComfyUI) | 任意（ローカル） | 任意 | 任意 | 無料 + GPU | 難しい |

---

## プロンプトコレクション

- ⭐ [NSFW AI Video Prompts](https://github.com/ristponex/nsfw-ai-video-prompts) - カテゴリ別に整理された100以上のコピー＆ペースト対応プロンプト
- ⭐ [Wan 2.2 Spicy Guide](https://github.com/ristponex/wan-spicy-nsfw-guide) - 完全なAPIサンプル付き50以上のプロンプト
- [Wan 2.2 Spicy LoRA Guide](https://github.com/ristponex/wan-2.2-spicy-lora-nsfw) - LoRA専用プロンプトとスタイルガイド
- [NSFW AI Image Prompts](https://github.com/ristponex/nsfw-ai-image-prompts) - 画像生成プロンプトライブラリ

---

## LoRAリソース

### NSFW LoRAの入手先

- [Civitai](https://civitai.com) - 最大のLoRAマーケットプレイス。NSFW、動画互換でフィルタリング可能。
- [HuggingFace](https://huggingface.co/models?other=lora) - オープンソースLoRAモデル
- [Tensor.Art](https://tensor.art) - プレビュー付きコミュニティLoRAギャラリー
- [AIBooru](https://aibooru.online) - リンク付きLoRAのAIアートギャラリー

### Wan 2.2 SpicyでLoRAを使う

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

## ツール

### 動画生成インターフェース

- [ComfyUI](https://github.com/comfyanonymous/ComfyUI) - ローカル生成用ノードベースワークフロー
- [A1111 WebUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui) - 定番のStable Diffusionインターフェース
- [Forge](https://github.com/lllyasviel/stable-diffusion-webui-forge) - 最適化されたA1111フォーク

### 動画エンハンスメント

- [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN) - 動画/画像アップスケーリング
- [GFPGAN](https://github.com/TencentARC/GFPGAN) - 顔の復元
- [FFmpeg](https://ffmpeg.org) - 動画処理、結合、音声マージ

### 音声同期

- [FFmpeg Audio Merge](https://ffmpeg.org) - `ffmpeg -i video.mp4 -i audio.mp3 -c copy output.mp4`
- Wan 2.6 / Seedance v1.5 — ネイティブ `generate_audio` パラメータ

---

## チュートリアル

### はじめに

1. **[Wan 2.2 Spicy完全ガイド](https://github.com/ristponex/wan-spicy-nsfw-guide)** — ゼロから5分で最初の動画を作成
2. **[LoRAガイド](https://github.com/ristponex/ai-video-lora-guide)** — LoRAアダプターによるカスタムスタイル
3. **[API比較](https://github.com/ristponex/nsfw-ai-api-comparison)** — 最適なプラットフォームを見つける

### プロンプトエンジニアリング

- 具体的な解剖学的・動作の記述を使用する
- ライティングを記述する："soft studio lighting"、"golden hour"、"rim lighting"
- カメラの方向："close-up"、"medium shot"、"slow pan"
- ネガティブプロンプト："blurry, distorted, watermark, text"

### リファレンス画像のコツ

- 高品質なソース画像を使用する（720p以上推奨）
- きれいな背景、良好なライティング、明確な被写体
- 必要に応じてFlux Devでリファレンス画像を生成する

---

## コミュニティ

### Reddit

- [r/AiNSFW](https://reddit.com/r/AiNSFW) - AI NSFW全般のディスカッション
- [r/unstable_diffusion](https://reddit.com/r/unstable_diffusion) - 無検閲AIアート
- [r/sdnsfw](https://reddit.com/r/sdnsfw) - Stable Diffusion NSFW
- [r/AIVideoGeneration](https://reddit.com/r/AIVideoGeneration) - AI動画のディスカッション

### Discord

- [Civitai Discord](https://discord.gg/civitai) - モデル共有とコツ
- [ComfyUI Discord](https://discord.gg/comfyui) - ワークフローのヘルプ

---

## モデル比較

| 機能 | Wan 2.2 Spicy | Wan 2.6 | Seedance 1.5 | Vidu Q3-Pro | セルフホスト |
|---------|:------------:|:-------:|:------------:|:-----------:|:-----------:|
| **NSFW品質** | ★★★★★ | ★★★★☆ | ★★★★☆ | ★★★★☆ | ★★★★★ |
| **価格** | $0.03/秒 | $0.04–0.15/秒 | $0.018–0.222 | $0.06–0.16/秒 | GPU費用 |
| **最大解像度** | 720p | 1080p | 720p | 1080p | 様々 |
| **最大長さ** | 8秒 | 15秒 | 5秒 | 可変 | 様々 |
| **音声** | ❌ | ✅ | ✅ | ✅ | 様々 |
| **LoRA** | ✅ | ❌ | ❌ | ❌ | ✅ |
| **アニメスタイル** | LoRA経由 | ❌ | ❌ | ✅ ネイティブ | ✅ |
| **テキストから動画** | ❌（I2Vのみ） | ✅ | ✅ | ✅ | ✅ |
| **セットアップ** | APIキー | APIキー | APIキー | APIキー | GPU + セットアップ |

---

## 法律と倫理

### 許容される使用

- 個人的な芸術表現
- ライセンスを取得した成人向けエンターテインメント制作
- 学術・研究目的
- ファッションおよびファインアート写真

### 厳禁事項

- 未成年者を含むコンテンツ（ゼロトレランス）
- 実在の人物の非同意ディープフェイク
- 地域の法律に違反するコンテンツ
- ハラスメントやリベンジコンテンツ

### ベストプラクティス

- すべての視聴者とユーザーの年齢を確認する
- 架空のキャラクターのみを使用するか、明示的な同意を得る
- AI生成コンテンツを明確にラベル付けする
- 管轄区域の法律を遵守する

---

## FAQ

<details>
<summary><b>NSFW動画を生成する最も安い方法は何ですか？</b></summary>
Atlas Cloud経由のWan 2.2 Spicyで$0.03/秒 — 5秒の動画がわずか$0.15です。
</details>

<details>
<summary><b>NSFW品質が最も高いモデルはどれですか？</b></summary>
Wan 2.2 Spicy（カスタムスタイル用のLoRAバリアント）。解剖学とモーションがファインチューニングされた成人向けコンテンツ専用に構築されています。
</details>

<details>
<summary><b>テキストからNSFW動画を生成できますか？</b></summary>
Wan 2.2 Spicyは画像から動画のみです。テキストからNSFW動画を生成するには、Wan 2.6 T2VまたはSeedance v1.5を使用してください。
</details>

<details>
<summary><b>NSFW AI動画の生成は合法ですか？</b></summary>
ほとんどの管轄区域では、架空のキャラクターのNSFWコンテンツを個人使用目的で生成することは合法です。常に地域の法律を確認してください。未成年者を含むコンテンツは絶対に作成しないでください。
</details>

<details>
<summary><b>強力なコンピュータが必要ですか？</b></summary>
いいえ — APIベースのサービスはクラウドGPU上で実行されます。インターネット接続とAPIキーがあれば十分です。
</details>

<details>
<summary><b>より良い結果を得るにはどうすればよいですか？</b></summary>
高品質なリファレンス画像、詳細なプロンプトを使用し、LoRAスタイルを試してみてください。上記のプロンプトコレクションをご参照ください。
</details>

---

## コントリビューション

新しいモデルを見つけましたか？便利なリソースがありますか？PRを開いてください！

- `- [名前](URL) - 説明` の形式に従う
- 価格と主要スペックを含める
- 提出前にリソースをテストする
- 説明は簡潔かつ事実に基づいたものにする

---

## ライセンス

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

法律の下で可能な限り、貢献者はこの作品に対するすべての著作権および関連する権利を放棄しています。
