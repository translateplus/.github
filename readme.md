# TranslatePlus - Real Time Translation API

<div align="center">

![TranslatePlus Logo](https://translateplus.io/assets/images/logo-dark.png)

**Fast, Affordable, and Reliable Translation API for Developers**

[![Website](https://img.shields.io/badge/Website-translateplus.io-purple)](https://translateplus.io)
[![API Docs](https://img.shields.io/badge/API-Documentation-blue)](https://docs.translateplus.io)
[![Trustpilot](https://img.shields.io/badge/Trustpilot-Reviews-green)](https://www.trustpilot.com/review/translateplus.io)
[![Chrome Extension](https://img.shields.io/badge/Chrome-Extension-orange)](https://chromewebstore.google.com/detail/translateplus/ijoblndpdmdobhmagcpoccipfgkjfjkp)

</div>

---

## 🚀 Why Choose TranslatePlus?

### ⚡ **Faster**
- **Sub-second response times** - Optimized infrastructure for lightning-fast translations
- **Async processing** - Handle large files and batch requests without blocking
- **Global CDN** - Low latency worldwide with distributed edge servers
- **Concurrent requests** - Built for high-volume usage

### 💰 **Cheaper**
- **Competitive pricing** - Up to 70% cheaper than major competitors
- **Transparent pricing** - No hidden fees, pay only for what you use
- **Flexible plans** - From free tier to enterprise solutions
- **Volume discounts** - Better rates for higher usage

### 🎯 **Better**
- **100+ languages** - Support for major world languages
- **High accuracy** - Powered by advanced neural machine translation
- **Developer-friendly** - Clean REST API with comprehensive documentation
- **Reliable uptime** - 99.9% SLA with enterprise-grade infrastructure

---

## ✨ Key Features

### Core Translation Capabilities

- **📝 Text Translation** - Translate text between 100+ languages with high accuracy
- **📦 Batch Translation** - Translate up to 100 texts in a single API call
- **🌐 Auto Language Detection** - Automatically detect source language
- **🌍 HTML Translation** - Translate HTML content while preserving all tags and structure
- **📧 Email Translation** - Translate email subjects and HTML bodies simultaneously
- **🎬 Subtitle Translation** - Translate SRT and VTT files with preserved timestamps

### Internationalization (i18n) Support

- **📄 Multi-format Support** - JSON, YAML, PO/POT, Properties, Strings, and XML files
- **🔧 Structure Preservation** - Maintains file structure, keys, placeholders, and formatting
- **⚙️ Background Processing** - Asynchronous job processing for large files
- **🔔 Webhook Notifications** - Receive notifications when translation jobs complete
- **🏷️ Placeholder Preservation** - All placeholders, ICU MessageFormat, and HTML/XML tags preserved

### Developer Experience

- **🔌 RESTful API** - Clean, intuitive REST API design
- **📚 Comprehensive Documentation** - Detailed API reference with code examples
- **💻 Multiple SDKs** - Code examples in cURL, Python, JavaScript, Node.js, and PHP
- **🛡️ Error Handling** - Standardized error messages with clear HTTP status codes
- **⚡ Rate Limiting** - Transparent rate limits with clear error messages

---

## 🚀 Quick Start

### Get Your API Key

1. Sign up at [translateplus.io](https://translateplus.io)
2. Get your API key from the dashboard
3. Start translating!

### Example Request

```bash
curl https://api.translateplus.io/v2/translate \
  -H "X-API-KEY: your_api_key" \
  -H "Content-Type: application/json" \
  -d '{
    "text": "Hello, world!",
    "source": "en",
    "target": "fr"
  }'
```

### Example Response

```json
{
  "translations": {
    "text": "Hello, world!",
    "translation": "Bonjour le monde!",
    "source": "en",
    "target": "fr"
  },
  "details": {}
}
```

---

## 📖 API Endpoints

### Translation Endpoints

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/v2/translate` | POST | Translate text from source to target language |
| `/v2/translate/batch` | POST | Translate multiple texts in a single request |
| `/v2/translate/html` | POST | Translate HTML content with structure preservation |
| `/v2/translate/subtitles` | POST | Translate subtitle files (SRT, VTT) |
| `/v2/translate/email` | POST | Translate email subjects and HTML bodies |
| `/v2/translate/i18n` | POST | Translate i18n files (JSON, YAML, PO, etc.) |
| `/v2/detect_language` | POST | Automatically detect source language |
| `/v2/supported-languages` | GET | Get list of supported languages |

### Account Management

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/v2/account` | GET | Get account information and usage stats |
| `/v2/account/credits` | GET | Check available credits |
| `/v2/account/usage` | GET | Get API usage statistics |

---

## 💻 Code Examples

### Python

```python
import requests

url = "https://api.translateplus.io/v2/translate"
headers = {
    "X-API-KEY": "your_api_key",
    "Content-Type": "application/json"
}
data = {
    "text": "Hello, world!",
    "source": "en",
    "target": "fr"
}

response = requests.post(url, json=data, headers=headers)
print(response.json())
```

### JavaScript

```javascript
fetch('https://api.translateplus.io/v2/translate', {
  method: 'POST',
  headers: {
    'X-API-KEY': 'your_api_key',
    'Content-Type': 'application/json'
  },
  body: JSON.stringify({
    text: 'Hello, world!',
    source: 'en',
    target: 'fr'
  })
})
.then(response => response.json())
.then(data => console.log(data))
.catch(error => console.error('Error:', error));
```

### Node.js

```javascript
const axios = require('axios');

axios.post('https://api.translateplus.io/v2/translate', {
  text: 'Hello, world!',
  source: 'en',
  target: 'fr'
}, {
  headers: {
    'X-API-KEY': 'your_api_key',
    'Content-Type': 'application/json'
  }
})
.then(response => console.log(response.data))
.catch(error => console.error('Error:', error));
```

---

## 🌍 Supported Languages

TranslatePlus supports **100+ languages** including:

- **European**: English, French, German, Spanish, Italian, Portuguese, Dutch, Russian, Polish, and more
- **Asian**: Chinese (Simplified & Traditional), Japanese, Korean, Hindi, Thai, Vietnamese, and more
- **Middle Eastern**: Arabic, Hebrew, Turkish, Persian, and more
- **African**: Swahili, Afrikaans, and more
- **And many more...**

See the full list at [Supported Languages](https://docs.translateplus.io/reference/v2/supported-languages)

---

## 📊 Pricing

### Why We're Cheaper

- **No setup fees** - Start translating immediately
- **Pay-as-you-go** - Only pay for what you use
- **Volume discounts** - Better rates for higher usage
- **No monthly minimums** - Perfect for small projects
- **Transparent pricing** - See exactly what you'll pay

*Note: Pricing may vary. Check our [pricing page](https://translateplus.io/pricing) for current rates.*

---

## 🔗 Resources

- **🌐 Website**: [translateplus.io](https://translateplus.io)
- **📚 API Documentation**: [docs.translateplus.io](https://docs.translateplus.io)
- **💬 Support**: [support@translateplus.io](mailto:support@translateplus.io)
- **⭐ Trustpilot Reviews**: [Review us on Trustpilot](https://www.trustpilot.com/review/translateplus.io)
- **🔌 Chrome Extension**: [Install from Chrome Web Store](https://chromewebstore.google.com/detail/translateplus/ijoblndpdmdobhmagcpoccipfgkjfjkp)

---

## 🛠️ Integration Examples

### Batch Translation

```bash
curl https://api.translateplus.io/v2/translate/batch \
  -H "X-API-KEY: your_api_key" \
  -H "Content-Type: application/json" \
  -d '{
    "texts": [
      "Hello, world!",
      "How are you?",
      "Thank you very much"
    ],
    "source": "en",
    "target": "fr"
  }'
```

### HTML Translation

```bash
curl https://api.translateplus.io/v2/translate/html \
  -H "X-API-KEY: your_api_key" \
  -H "Content-Type: application/json" \
  -d '{
    "html": "<p>Hello, <strong>world</strong>!</p>",
    "source": "en",
    "target": "fr"
  }'
```

### Subtitle Translation

```bash
curl https://api.translateplus.io/v2/translate/subtitles \
  -H "X-API-KEY: your_api_key" \
  -H "Content-Type: application/json" \
  -d '{
    "subtitle": "1\n00:00:00,000 --> 00:00:02,000\nHello, world!",
    "format": "srt",
    "source": "en",
    "target": "fr"
  }'
```

---

## 🎯 Use Cases

- **🌐 Website Localization** - Translate your website content into multiple languages
- **📱 Mobile Apps** - Integrate translation into iOS and Android apps
- **📧 Email Marketing** - Send multilingual email campaigns
- **🎬 Video Content** - Translate subtitles for video content
- **📄 Documentation** - Translate technical documentation
- **💬 Customer Support** - Provide multilingual customer support
- **🛒 E-commerce** - Translate product descriptions and reviews
- **📊 Analytics** - Translate user-generated content for analysis

---

## 🔒 Security & Reliability

- **🔐 API Key Authentication** - Secure API key-based authentication
- **🛡️ HTTPS Only** - All API calls encrypted with TLS 1.3
- **📊 Rate Limiting** - Protect your account from abuse
- **✅ 99.9% Uptime SLA** - Enterprise-grade reliability
- **🔍 Request Logging** - Track all API requests for debugging
- **📈 Usage Analytics** - Monitor your API usage in real-time

---

## 📈 Performance Benchmarks

- **Average Response Time**: < 500ms
- **P95 Response Time**: < 1s
- **Throughput**: 1000+ requests/second
- **Uptime**: 99.9% SLA
- **Supported Languages**: 100+

---

## 🤝 Support

- **📧 Email**: [support@translateplus.io](mailto:support@translateplus.io)
- **💬 Live Chat**: Available on [translateplus.io](https://translateplus.io)
- **📚 Documentation**: [docs.translateplus.io](https://docs.translateplus.io)
- **🐛 Issues**: Report issues via email or our support portal

---

## 📄 License

Copyright © 2024 TranslatePlus. All rights reserved.

---

<div align="center">

**Made with ❤️ for developers**

[Get Started](https://translateplus.io) • [Documentation](https://docs.translateplus.io) • [Support](mailto:support@translateplus.io)

</div>

