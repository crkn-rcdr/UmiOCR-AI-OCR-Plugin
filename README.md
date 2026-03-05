# Umi-OCR AI OCR Plugin

## 🚀 Project Introduction

This plugin provides **OCR functionality from 14 major mainstream AI
service providers** for **Umi-OCR**, supporting both cloud and local AI
visual recognition APIs. As a powerful supplement to offline OCR, it
delivers higher accuracy and broader language support for intelligent
text recognition.

------------------------------------------------------------------------

## 📋 About Umi-OCR

**Umi-OCR** is a free, open-source, batch-capable offline OCR software
built on PaddleOCR. It has the following features:

GitHub stars \| License \| Python \| Multi-AI

-   🆓 Completely Free: No payment required, no ads, open-source
    software\
-   📱 User-Friendly Interface: Modern graphical interface, simple and
    intuitive\
-   🔄 Batch Processing: Supports batch image OCR to improve efficiency\
-   🌐 Multi-language Support: Supports Chinese, English, Japanese,
    Korean, and more\
-   🔌 Plugin System: Supports extension plugins with customizable
    functionality\
-   💻 Cross-platform: Supports Windows, Linux, and other operating
    systems

------------------------------------------------------------------------

# 🌟 Supported AI Service Providers

## 🌐 Cloud Providers

  ---------------------------------------------------------------------------------------
  Provider             Recommended Model                               Features
  -------------------- ----------------------------------------------- ------------------
  SiliconFlow          Qwen/Qwen3-VL-235B-A22B-Instruct (recommended)  Many open-source
                       or Qwen/Qwen2.5-VL-72B-Instruct                 models, low cost,
                                                                       fast speed,
                                                                       extremely high
                                                                       accuracy, **most
                                                                       recommended**

  Alibaba Bailian      Qwen/Qwen3-VL-235B-A22B-Instruct                Top-tier OCR
                                                                       model, excellent
                                                                       Chinese
                                                                       recognition,
                                                                       **most
                                                                       recommended**

  ZhipuAI              glm-4.5v                                        Domestic large
                                                                       model, strong
                                                                       multimodal
                                                                       capability

  Doubao               doubao-seed-1-6-vision-250815                   Optimized for
                                                                       Chinese, high
                                                                       cost-performance

  OpenAI               gpt-5-mini                                      High accuracy,
                                                                       multilingual
                                                                       support

  Google Gemini        gemini-3.0-flash                                Fast speed, low
                                                                       cost

  xAI Grok             grok-4                                          Innovative model
                                                                       with unique
                                                                       advantages

  OpenRouter           qwen/qwen2.5-vl-72b-instruct:free               Unified interface,
                                                                       rich model
                                                                       selection

  Groq                 meta-llama/llama-4-maverick-17b-128e-instruct   High-performance
                                                                       inference,
                                                                       extremely fast

  ModelScope           Qwen/Qwen3-VL-235B-A22B-Instruct                Alibaba DAMO
                                                                       open-source
                                                                       platform, rich
                                                                       models, free usage

  Infinigence          Qwen/Qwen3-VL-235B-A22B-Instruct                Top-tier OCR
                                                                       model, excellent
                                                                       Chinese
                                                                       recognition, free
                                                                       usage

  Mistral AI           mistral-ocr-latest                              European AI
                                                                       company, strong
                                                                       vision models,
                                                                       free usage

  Intern               internvl3.5-241b-a28b                           Academic AI
                                                                       platform, strong
                                                                       multimodal
                                                                       capability, free
                                                                       usage

  PaddleOCR Series     V3/V5/VL                                        Baidu Paddle
                                                                       platform,
                                                                       multilingual
                                                                       recognition,
                                                                       efficient and
                                                                       accurate document
                                                                       parsing
  ---------------------------------------------------------------------------------------

------------------------------------------------------------------------

## 🏠 Local Providers (Offline Recognition)

  --------------------------------------------------------------------------
  Provider             Recommended Model                Features
  -------------------- -------------------------------- --------------------
  Ollama               qwen2.5vl:7b, qwen3vl:8b         🔒 Fully offline,
                                                        privacy protection,
                                                        free usage, supports
                                                        custom address

  LM Studio            llava, llava-1.5-7b-hf           🔒 Fully offline,
                                                        user-friendly GUI,
                                                        OpenAI-compatible,
                                                        supports custom
                                                        address
  --------------------------------------------------------------------------

### 💡 Custom Address Feature

Ollama and LM Studio support custom API addresses. You can:

-   🌐 Connect to Ollama/LM Studio services on other machines within
    your LAN\
-   ⚡ Run Umi-OCR on lower-spec hardware while connecting to a
    high-performance AI service machine\
-   🔧 Deploy flexibly and fully utilize existing hardware resources\
-   📡 Support remote AI services for distributed OCR processing

------------------------------------------------------------------------

# 📊 Recognition Comparison

### Settings Interface

Settings interface

### Recognition Image: "Even extremely complex handwritten information can be perfectly recognized"

Recognition image

### PaddleOCR Recognition Result --- Very Poor

PaddleOCR recognition result, very poor

### WechatOCR Recognition Result --- Very Poor

WechatOCR recognition result, very poor

### AI OCR (Model: Gemini 2.5 Flash) Recognition Result --- Nearly Perfect

AI OCR recognition result, perfect!

image image

------------------------------------------------------------------------

# ✨ Features

  -----------------------------------------------------------------------
  Feature                        Description
  ------------------------------ ----------------------------------------
  🚀 High-Accuracy Recognition   Based on the latest AI vision models,
                                 supports multi-language text recognition

  🌍 Multi-language Support      Supports Chinese, English, Japanese,
                                 Korean, French, German, Spanish,
                                 Russian, Arabic, etc.

  ⚡ Multiple Provider Options   Supports OpenAI, Gemini, xAI,
                                 OpenRouter, SiliconFlow, Doubao, and
                                 more

  📍 Coordinate Extraction       Optional output of text position
                                 coordinate information

  🔧 Flexible Configuration      Supports adjustment of image quality,
                                 size, timeout, and other parameters

  🌐 Proxy Support               Supports HTTP/SOCKS5 proxy

  🔄 Smart Retry                 Automatic retry mechanism to improve
                                 recognition success rate

  🚀 Concurrent Processing       Supports concurrent batch image
                                 recognition to improve efficiency
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# 📦 Installation Requirements

-   Umi-OCR software: Install Umi-OCR v2.0+\
-   AI service API key: Obtain API keys from corresponding providers\
-   Network connection: Must be able to access the AI services (overseas
    models typically require VPN access)

------------------------------------------------------------------------

# 🛠️ Installation Steps

-   Download the latest plugin version from AIOCR-releases\
-   Extract the AIOCR folder into the Umi-OCR plugin directory:

```{=html}
<!-- -->
```
    UmiOCR-data/plugins/

-   Restart Umi-OCR\
-   Select "AI OCR (Cloud)" in the OCR engine selection

------------------------------------------------------------------------

# ⚙️ Configuration Instructions

## 1. Configure the Plugin

### First-time Configuration (recommended to configure all providers at once):

-   Select "AI OCR (Cloud)" in Umi-OCR\
-   Configure all providers you plan to use in Global Settings:
    -   Enter OpenAI API key and model (if needed)\
    -   Enter Gemini API key and model (if needed)\
    -   Configure other providers (if needed)\
-   Select the current AI provider and click **Apply Changes**\
-   In Local Settings, choose "Recognition Strategy":
    -   Dual-channel: AI high-accuracy recognition (with position):
        Outputs text with coordinates, suitable for PDF and document
        recognition.\
    -   AI high-accuracy recognition only: Outputs plain text without
        coordinates, suitable when only text is needed.\
-   Set parameters:
    -   Edge padding: 2 px\
    -   Maximum detection boxes: 30--100 (balance complexity and cost)\
    -   Concurrent recognition: 3--6 (depending on machine and provider
        rate limits)\
    -   Minimum box area: 0 or 100--500 px² (0 recommended for small
        text scenarios)

image

### Daily Use:

-   Simply switch the "Current AI Provider" dropdown and click **Apply
    Changes**\
-   No need to re-enter API keys or models\
-   All configurations are saved automatically

------------------------------------------------------------------------

## 2. Start Recognition

-   Use screenshot OCR, batch OCR, and other functions\
-   The plugin will automatically call the corresponding AI API for
    recognition

------------------------------------------------------------------------

# ⚠️ Notes

-   API Cost: AI APIs are billed by usage. Please control frequency.\
-   Network Requirement: Requires stable internet connection.\
-   Image Size: Set an appropriate maximum image size to control cost.\
-   Privacy & Security: Images are uploaded directly to provider
    servers. The plugin author does not receive your images or data.\
-   Speed Limits: Cloud APIs may have rate limits and are not suitable
    for excessive concurrent requests.\
-   Model Selection: Accuracy and cost vary by model. Choose based on
    your needs.\
-   Chinese Variant Preservation: When language is set to
    "Auto/Chinese", simplified/traditional conversion,
    full-width/half-width conversion, and character normalization are
    explicitly prohibited; mixed variants remain mixed; characters are
    copied verbatim without rewriting.

------------------------------------------------------------------------

# 🔑 API Key Acquisition

## SiliconFlow

-   Visit SiliconFlow\
-   Register an account and obtain API key\
-   Supports multiple open-source vision models

## Doubao

-   Visit Volcano Engine\
-   Activate Doubao service and obtain API key\
-   ByteDance-developed multimodal model

## OpenAI

-   Visit OpenAI Platform\
-   Log in and create API key\
-   Copy generated key

## Google Gemini

-   Visit Google AI Studio\
-   Log in with Google account\
-   Create new API key

## xAI Grok

-   Visit xAI Console\
-   Register and obtain API key

## Alibaba Bailian

-   Visit Alibaba Bailian Platform\
-   Activate service and obtain API key\
-   Supports Tongyi Qwen vision models

## ZhipuAI

-   Visit ZhipuAI Open Platform\
-   Register and create API key\
-   Domestic multimodal large model

## OpenRouter

-   Visit OpenRouter\
-   Register and create API key

## Groq

-   Visit Groq Console\
-   Register and obtain API key\
-   High-performance inference platform

## ModelScope

-   Visit ModelScope Community\
-   Register and obtain Access Token\
-   Alibaba DAMO open-source AI platform

## Infinigence

-   Visit Infinigence Platform\
-   Register and obtain API key\
-   Moonshot AI platform with strong long-text capability

## Mistral AI

-   Visit Mistral Platform\
-   Register and create API key\
-   European AI company with strong vision models

## Intern

-   Visit InternLM Platform\
-   Register and obtain API key\
-   Academic AI platform with strong multimodal capability

## Baidu PaddleOCR

-   Visit PaddleOCR official site: https://aistudio.baidu.com/paddleocr\
-   Register and obtain TOKEN and API_URL for free\
-   Daily limit: 3000 pages per model per user; exceeding returns HTTP
    429

------------------------------------------------------------------------

# 🏠 Local Service Installation Guide

## Ollama (Fully Offline)

### Install Ollama

``` bash
# Linux/macOS
curl -fsSL https://ollama.ai/install.sh | sh

# Windows
# Download installer from https://ollama.ai
```

### Download Vision Models

``` bash
# Download llava model (recommended)
ollama pull llava

# Or download other vision models
ollama pull llava:7b
ollama pull bakllava
```

### Start Service

``` bash
ollama serve
# Service will start at http://localhost:11434
```

### Configure in Plugin

-   Provider: Select "Ollama (Local)"\
-   Model: Enter downloaded model name (e.g., llava)\
-   Default API address (editable): http://localhost:11434/api\
-   API key: Leave blank

------------------------------------------------------------------------

## LM Studio (GUI)

### Install

-   Visit LM Studio official website\
-   Download and install version for your system

### Download Models

-   Search and download vision-supported models inside LM Studio\
-   Recommended: llava-1.5-7b-hf, llava-1.6-34b-hf

### Start Local Server

-   Click "Local Server" in LM Studio\
-   Select downloaded vision model\
-   Start server (default port 1234)

### Configure in Plugin

-   Provider: Select "LM Studio (Local)"\
-   Model: Enter model name loaded in LM Studio\
-   Default API address (editable): http://localhost:1234/v1\
-   API key: Leave blank or enter "not-needed"

------------------------------------------------------------------------

# 🔒 Advantages of Local Services

-   Fully offline: No internet required, no data uploaded\
-   Privacy protection: All processing happens locally\
-   Free usage: No API call cost\
-   Full control: Choose and customize models

------------------------------------------------------------------------

# 📝 Version History

-   v2.9.1: Added PaddleOCR-VL-1.5, improved performance\
-   v2.9.0: Added PP-StructureV3 for more accurate complex layout
    parsing. Layout recognition and Markdown beautification enabled by
    default.\
-   v2.8.0: Added PaddleOCR-V5 and PaddleOCR-VL\
-   v2.7.0: Adjusted dual-channel strategy, improved accuracy and speed\
-   v2.6.0: 🚀 Major update --- solved large-model OCR text alignment
    issue. Added and improved dual-channel recognition. Local PaddleOCR
    detects real coordinates; AI model recognizes text for perfect
    alignment. Adjustable concurrency, box limit, padding, etc. Faster
    full-image recognition.\
-   v2.5.0: 🎉 Community update --- added 5 AI providers: Groq,
    ModelScope, Infinigence, Mistral AI, Intern. Expanded provider
    selection. Optimized local custom address feature.\
-   v2.4.0: 🚀 Major update --- added local offline recognition (Ollama,
    LM Studio). Custom API address supported. Improved text alignment
    accuracy.\
-   v2.3.0: Added Alibaba Bailian and ZhipuAI support. Updated default
    models. Optimized UI. Removed retry count config (built-in 3
    retries).\
-   v2.2.0: One-time configuration for all providers. No need to
    re-enter API keys when switching.\
-   v2.1.0: Added SiliconFlow and Doubao vision models\
-   v2.0.0: Refactored into multi-provider AI OCR plugin\
-   v1.2.0: Added Gemini 2.5 Flash and Pro preview models, improved
    recognition accuracy\
-   v1.1.0: Added multi-language support, optimized error handling\
-   v1.0.0: Initial release with Gemini OCR support

------------------------------------------------------------------------

# 💖 Support

If this plugin helps you, please consider:

-   Giving the project a ⭐\
-   Sharing it with others\
-   Providing feedback and suggestions\
-   Contributing to the project

------------------------------------------------------------------------

**Thank you for using the Umi-OCR Multi-Provider AI OCR Plugin!**
