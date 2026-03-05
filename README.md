# Umi-OCR AI OCR Plugin

## 🚀 Project Introduction

This plugin provides **OCR functionality from 14 major AI service
providers** for **Umi-OCR**, supporting both cloud-based and local AI
visual recognition APIs. As a powerful supplement to offline OCR, it
offers higher accuracy and broader language support for intelligent text
recognition.

------------------------------------------------------------------------

## 📋 About Umi-OCR

**Umi-OCR** is a free, open-source, batch-capable offline OCR software
built on PaddleOCR. It has the following features:

-   🆓 **Completely Free**: No payment required, no ads, open-source
    software\
-   📱 **User-Friendly Interface**: Modern graphical interface, simple
    and intuitive\
-   🔄 **Batch Processing**: Supports batch image OCR to improve
    efficiency\
-   🌐 **Multi-language Support**: Supports Chinese, English, Japanese,
    Korean, and more\
-   🔌 **Plugin System**: Extensible plugin support with customizable
    features\
-   💻 **Cross-platform**: Supports Windows, Linux, and other operating
    systems

------------------------------------------------------------------------

## 🌟 Supported AI Service Providers

### 🌐 Cloud Providers

  -------------------------------------------------------------------------------------
  Provider           Recommended Model                               Features
  ------------------ ----------------------------------------------- ------------------
  SiliconFlow        Qwen/Qwen3-VL-235B-A22B-Instruct (recommended)  Many open-source
                     or Qwen/Qwen2.5-VL-72B-Instruct                 models, low price,
                                                                     fast speed,
                                                                     extremely high
                                                                     accuracy, **most
                                                                     recommended**

  Alibaba Bailian    Qwen/Qwen3-VL-235B-A22B-Instruct                Top-tier OCR
                                                                     model, excellent
                                                                     Chinese
                                                                     recognition,
                                                                     **highly
                                                                     recommended**

  ZhipuAI            glm-4.5v                                        Domestic large
                                                                     model, strong
                                                                     multimodal
                                                                     capability

  Doubao             doubao-seed-1-6-vision-250815                   Optimized for
                                                                     Chinese, high
                                                                     cost-performance

  OpenAI             gpt-5-mini                                      High precision,
                                                                     multilingual
                                                                     support

  Google Gemini      gemini-3.0-flash                                Fast speed, low
                                                                     cost

  xAI Grok           grok-4                                          Innovative model
                                                                     with unique
                                                                     advantages

  OpenRouter         qwen/qwen2.5-vl-72b-instruct:free               Unified interface,
                                                                     rich model
                                                                     selection

  Groq               meta-llama/llama-4-maverick-17b-128e-instruct   High-performance
                                                                     inference,
                                                                     extremely fast

  ModelScope         Qwen/Qwen3-VL-235B-A22B-Instruct                Alibaba DAMO
                                                                     open-source
                                                                     platform, rich
                                                                     models, free usage

  Infinigence        Qwen/Qwen3-VL-235B-A22B-Instruct                Top-tier OCR
                                                                     model, excellent
                                                                     Chinese
                                                                     recognition, free
                                                                     usage

  Mistral AI         mistral-ocr-latest                              European AI
                                                                     company, strong
                                                                     vision models,
                                                                     free usage

  Intern             internvl3.5-241b-a28b                           Academic AI
                                                                     platform, strong
                                                                     multimodal
                                                                     capability, free
                                                                     usage

  PaddleOCR Series   V3/V5/VL                                        Baidu Paddle
                                                                     platform,
                                                                     multilingual
                                                                     recognition,
                                                                     efficient document
                                                                     parsing
  -------------------------------------------------------------------------------------

------------------------------------------------------------------------

### 🏠 Local Providers (Offline Recognition)

  -------------------------------------------------------------------------
  Provider           Recommended Model                 Features
  ------------------ --------------------------------- --------------------
  Ollama             qwen2.5vl:7b, qwen3vl:8b          🔒 Fully offline,
                                                       privacy protection,
                                                       free, **supports
                                                       custom API address**

  LM Studio          llava, llava-1.5-7b-hf            🔒 Fully offline,
                                                       user-friendly GUI,
                                                       OpenAI-compatible,
                                                       **supports custom
                                                       API address**
  -------------------------------------------------------------------------

> 💡 **Custom Address Feature**: Ollama and LM Studio support custom API
> addresses. You can:\
> - 🌐 Connect to Ollama/LM Studio services on other machines within
> your LAN\
> - ⚡ Run Umi-OCR on lower-spec hardware while connecting to a
> high-performance AI server\
> - 🔧 Deploy flexibly and fully utilize existing hardware resources\
> - 📡 Support remote AI services for distributed OCR processing

------------------------------------------------------------------------

## 📊 Recognition Comparison

### Settings Interface

### Recognition Example: "Even extremely complex handwritten information can be perfectly recognized"

### PaddleOCR Recognition Result -- Very Poor

### WeChat OCR Recognition Result -- Very Poor

### AI OCR (Model: Gemini 2.5 Flash) Recognition Result -- Nearly Perfect

------------------------------------------------------------------------

## ✨ Features

  -----------------------------------------------------------------------
  Feature                        Description
  ------------------------------ ----------------------------------------
  🚀 High-Accuracy Recognition   Based on the latest AI vision models,
                                 supports multiple languages

  🌍 Multi-language Support      Chinese, English, Japanese, Korean,
                                 French, German, Spanish, Russian,
                                 Arabic, etc.

  ⚡ Multiple Provider Options   Supports OpenAI, Gemini, xAI,
                                 OpenRouter, SiliconFlow, Doubao, etc.

  📍 Coordinate Extraction       Optional output of text position
                                 coordinate information

  🔧 Flexible Configuration      Adjustable image quality, size, timeout,
                                 and other parameters

  🌐 Proxy Support               Supports HTTP/SOCKS5 proxy

  🔄 Smart Retry                 Automatic retry mechanism to improve
                                 success rate

  🚀 Concurrent Processing       Supports concurrent batch image
                                 recognition
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## 📦 Installation Requirements

1.  **Umi-OCR Software**: Install Umi-OCR v2.0+\
2.  **AI Service API Key**: Obtain API keys from corresponding
    providers\
3.  **Network Connection**: Required for cloud AI services (overseas
    models may require VPN access)

------------------------------------------------------------------------

## 🛠️ Installation Steps

1.  Download the latest plugin release\

2.  Extract the `AIOCR` folder into:

    UmiOCR-data/plugins/

3.  Restart Umi-OCR\

4.  Select "AI OCR (Cloud)" in the OCR engine selection

------------------------------------------------------------------------

## ⚙️ Configuration Instructions

### 1. Configure the Plugin

**First-time Setup (Recommended to configure all providers at once):**

1.  Select "AI OCR (Cloud)" in Umi-OCR\
2.  Configure all providers you plan to use in Global Settings:
    -   Enter OpenAI API key and model (if needed)\
    -   Enter Gemini API key and model (if needed)\
    -   Configure other providers (if needed)\
3.  Select the current AI provider and click **Apply Changes**\
4.  Choose recognition strategy in Local Settings:
    -   Dual-channel: AI high-accuracy recognition (with position):
        Outputs text with coordinates, suitable for PDF documents\
    -   AI high-accuracy recognition only: Outputs plain text only\
5.  Parameter recommendations:
    -   Edge padding: 2 px\
    -   Maximum detection boxes: 30--100\
    -   Concurrent recognition: 3--6\
    -   Minimum box area: 0 or 100--500 px²

**Daily Usage:**

-   Simply switch providers from the dropdown and click **Apply
    Changes**\
-   No need to re-enter API keys\
-   All settings are automatically saved

------------------------------------------------------------------------

## ⚠️ Notes

1.  **API Costs**: Billed based on usage\
2.  **Network Requirement**: Stable connection required\
3.  **Image Size**: Adjust maximum image size to control cost\
4.  **Privacy**: Images are uploaded directly to provider servers;
    plugin author does not access your data\
5.  **Speed Limits**: Cloud APIs may have rate limits\
6.  **Model Selection**: Accuracy and cost vary by model\
7.  **Chinese Variant Preservation**: No automatic
    simplified/traditional conversion or normalization

------------------------------------------------------------------------

## 🔑 API Key Acquisition

Obtain API keys from the respective official platforms of each provider.

------------------------------------------------------------------------

## 🏠 Local Service Installation Guide

### Ollama (Fully Offline)

1.  Install Ollama\
2.  Download vision models\
3.  Start service (`ollama serve`)\
4.  Configure in plugin:
    -   Provider: Ollama (Local)\
    -   Model: downloaded model name\
    -   API address: http://localhost:11434/api\
    -   API key: leave blank

### LM Studio (GUI)

1.  Install LM Studio\
2.  Download vision models\
3.  Start local server (default port 1234)\
4.  Configure in plugin:
    -   Provider: LM Studio (Local)\
    -   Model: loaded model name\
    -   API address: http://localhost:1234/v1\
    -   API key: leave blank or "not-needed"

### 🔒 Advantages of Local Services

-   Fully offline\
-   Privacy protection\
-   Free usage\
-   Full model control

------------------------------------------------------------------------

## 📝 Version History

-   v2.9.1: Added PaddleOCR-VL-1.5\
-   v2.9.0: Added PP-StructureV3 layout parsing\
-   v2.8.0: Added PaddleOCR-V5 and PaddleOCR-VL\
-   v2.7.0: Improved dual-channel strategy\
-   v2.6.0: Major update -- solved text alignment issue\
-   v2.5.0: Added 5 AI providers\
-   v2.4.0: Added local offline recognition support\
-   v2.3.0: Added Alibaba Bailian and ZhipuAI support\
-   v2.2.0: One-time configuration for all providers\
-   v2.1.0: Added SiliconFlow and Doubao\
-   v2.0.0: Refactored to multi-provider AI OCR plugin\
-   v1.2.0: Added Gemini 2.5 Flash and Pro preview models\
-   v1.1.0: Added multi-language support\
-   v1.0.0: Initial release

------------------------------------------------------------------------

## 💖 Support

If this plugin helps you:

-   ⭐ Star the project\
-   Share it\
-   Provide feedback and suggestions\
-   Contribute to the project

------------------------------------------------------------------------

**Thank you for using the Umi-OCR Multi-Provider AI OCR Plugin!**
