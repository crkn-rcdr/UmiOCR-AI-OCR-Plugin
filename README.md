# Umi-OCR AI OCR Plugin

## 🚀 Project Introduction

This plugin provides OCR functionality from **14 major AI service providers** for Umi-OCR, supporting both cloud-based and local AI visual recognition APIs.

As a powerful supplement to offline OCR, it delivers higher accuracy and broader language support for intelligent text recognition.

---

## 📋 About Umi-OCR

Umi-OCR is a free, open-source, batch-capable offline OCR software built on PaddleOCR.

### Key Features

- 🆓 Completely free (no ads, open-source)
- 📱 Modern, user-friendly interface
- 🔄 Batch image OCR processing
- 🌐 Multi-language support
- 🔌 Plugin system (extendable)
- 💻 Cross-platform (Windows, Linux)

---

## 🌟 Supported AI Providers

### 🌐 Cloud Providers

| Provider | Recommended Model | Highlights |
|-----------|-------------------|------------|
| SiliconFlow | Qwen3-VL-235B-A22B-Instruct | Low cost, fast, extremely high accuracy |
| Alibaba Bailian | Qwen3-VL-235B-A22B-Instruct | Excellent Chinese OCR |
| ZhipuAI | glm-4.5v | Strong multimodal capabilities |
| Doubao | doubao-seed-1-6-vision | Optimized for Chinese |
| OpenAI | gpt-5-mini | High precision, multilingual |
| Google Gemini | gemini-3.0-flash | Fast and cost-efficient |
| xAI Grok | grok-4 | Advanced multimodal model |
| OpenRouter | qwen2.5-vl-72b-instruct | Unified API gateway |
| Groq | llama-4-maverick-17b | Ultra-fast inference |
| ModelScope | Qwen3-VL | Rich open model ecosystem |
| Infinigence | Qwen3-VL | Strong Chinese OCR |
| Mistral AI | mistral-ocr-latest | High-quality vision model |
| Intern | internvl3.5 | Academic multimodal platform |
| PaddleOCR Series | V3 / V5 / VL | Efficient structured document parsing |

---

### 🏠 Local Providers (Offline OCR)

| Provider | Recommended Model | Highlights |
|-----------|-------------------|------------|
| Ollama | qwen2.5vl / qwen3vl | Fully offline, privacy-first |
| LM Studio | llava / llava-1.5 | GUI-based, OpenAI-compatible |

### Custom API Address Support

Ollama and LM Studio support custom API endpoints, allowing:

- LAN-based AI services
- Remote high-performance servers
- Distributed OCR workflows
- Flexible deployment

---

## ✨ Features

- 🚀 High-precision AI recognition
- 🌍 Multi-language support (Chinese, English, Japanese, Korean, French, German, Spanish, Russian, Arabic, etc.)
- ⚡ Multi-vendor switching
- 📍 Optional coordinate extraction
- 🔧 Adjustable parameters (image size, timeout, detection count)
- 🌐 HTTP / SOCKS5 proxy support
- 🔄 Automatic retry mechanism
- 🚀 Concurrent batch processing

---

## 📦 Installation Requirements

1. Umi-OCR v2.0+
2. API key from selected AI provider
3. Stable internet connection (for cloud models)

---

## 🛠 Installation

1. Download the latest release:
   https://github.com/EatWorld/UmiOCR-AI-OCR-Plugin/releases

2. Extract the `AIOCR` folder into:

   ```
   UmiOCR-data/plugins/
   ```

3. Restart Umi-OCR.

4. Select **AI OCR (Cloud)** from the OCR engine list.

---

## ⚙️ Configuration

### First-Time Setup

1. Select **AI OCR (Cloud)**.
2. Enter API keys and model names in Global Settings.
3. Click **Apply Changes**.
4. Choose recognition strategy:

- **Dual-channel (AI High Precision + Coordinates)**  
  Suitable for PDFs and structured documents.

- **AI High Precision Only**  
  Outputs plain text without coordinates.

### Recommended Parameters

- Edge padding: 2 px  
- Max detection boxes: 30–100  
- Concurrent tasks: 3–6  
- Minimum box area: 0 (recommended for small text)

---

### Daily Usage

- Switch provider from dropdown.
- Click **Apply Changes**.
- No need to re-enter API keys.

All settings are automatically saved.

---

## ⚠️ Important Notes

- API usage is billed by providers.
- Stable network required for cloud OCR.
- Large images increase cost.
- Images are sent directly to provider servers.
- Cloud APIs may enforce rate limits.
- Different models vary in cost and accuracy.

### Chinese Variant Preservation

When language is set to “Auto/Chinese”:

- No Simplified/Traditional conversion
- No full-width/half-width conversion
- No character normalization
- Mixed variants remain unchanged

---

## 🏠 Local Offline Setup

### Ollama

Install:

```bash
curl -fsSL https://ollama.ai/install.sh | sh
```

Download model:

```bash
ollama pull llava
```

Start service:

```bash
ollama serve
```

Plugin Configuration:

- Provider: Ollama (Local)
- API: http://localhost:11434/api
- API Key: Leave blank

---

### LM Studio

1. Install from https://lmstudio.ai
2. Download a vision model (e.g., llava-1.5-7b-hf)
3. Start local server (default port 1234)

Plugin Configuration:

- Provider: LM Studio (Local)
- API: http://localhost:1234/v1
- API Key: blank or `not-needed`

---

## 🔒 Advantages of Local OCR

- Fully offline
- Privacy protected
- No API cost
- Full control over models

---

## 📝 Version History

- v2.9.1 — Added PaddleOCR-VL-1.5
- v2.9.0 — Added PP-StructureV3
- v2.8.0 — Added PaddleOCR-V5 and VL
- v2.7.0 — Improved dual-channel speed and accuracy
- v2.6.0 — Fixed alignment using dual-channel recognition
- v2.5.0 — Added 5 new AI providers
- v2.4.0 — Added local offline OCR support
- v2.3.0 — Added Alibaba Bailian and ZhipuAI
- v2.2.0 — One-time configuration for all providers
- v2.1.0 — Added SiliconFlow and Doubao
- v2.0.0 — Multi-provider refactor
- v1.2.0 — Gemini 2.5 support
- v1.1.0 — Improved multilingual handling
- v1.0.0 — Initial release

---

## 💖 Support

Head to source repo to support: https://github.com/EatWorld/UmiOCR-AI-OCR-Plugin

---

**Thank you for using the Umi-OCR Multi-Provider AI OCR Plugin!**
