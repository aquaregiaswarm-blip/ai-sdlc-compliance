# Data Handling Comparison

## Overview

This document compares how AI coding tools handle your code and data.

---

## Code Sent to Cloud

| Tool | Code Leaves Your Environment | Opt-Out Available | Zero Data Retention |
|------|------------------------------|-------------------|---------------------|
| **GitHub Copilot** | ✅ Yes | ✅ Enterprise opt-out | ❌ No |
| **Cursor** | ✅ Yes | ✅ Enterprise opt-out | ❌ No |
| **Windsurf** | ✅ Yes | ✅ Enterprise opt-out | ❌ No |
| **OpenAI Codex** | ✅ Yes | ✅ API option | ✅ API available |
| **Claude Code** | ✅ Yes | ✅ API option | ✅ API available |
| **Gemini Code Assist** | ✅ Yes | ✅ Enterprise controls | ❌ No |
| **Kiro (AWS)** | ✅ Yes | ✅ Enterprise controls | ✅ Available |
| **Tabnine** | ⚠️ Optional | ✅ Self-hosted option | ✅ Enterprise |
| **AWS Bedrock** | ✅ Yes | ✅ Configurable | ✅ Available |
| **Vertex AI** | ✅ Yes | ✅ Configurable | ✅ Available |
| **Azure Foundry** | ✅ Yes | ✅ Configurable | ✅ Available |

---

## Data Retention Policies

### GitHub Copilot
- **Prompts/Completions:** May be retained for product improvement
- **Opt-out:** Enterprise customers can opt-out of retention
- **Retention Period:** Not publicly specified
- **Location:** Global CDN, EU option available

### Cursor
- **Code Snippets:** Sent to cloud for processing
- **Opt-out:** Enterprise plans offer data controls
- **Retention:** Limited retention for service improvement
- **Location:** US-based infrastructure

### Windsurf/Codeium
- **Code:** Processed in cloud
- **Opt-out:** Enterprise customers can request no retention
- **Self-hosted:** On-premise option available
- **Location:** US and EU options

### OpenAI Codex
- **API:** Zero data retention option available
- **Retention:** Configurable via API settings
- **Enterprise:** Custom data handling agreements
- **Location:** US, EU options available

### Claude Code
- **API:** Zero data retention available
- **Retention:** Configurable
- **Enterprise:** Custom agreements
- **Location:** US, with EU coming

### Gemini Code Assist
- **Google Cloud:** Standard GCP data handling
- **Retention:** Configurable via workspace settings
- **Enterprise:** Custom data residency
- **Location:** Global, data residency options

### Kiro (AWS)
- **AWS:** Standard AWS data protection
- **Retention:** Configurable
- **GovCloud:** Available for government
- **Location:** AWS regions worldwide

### Tabnine
- **Cloud:** Basic plan sends code to cloud
- **Self-hosted:** Enterprise can run on-premise
- **Zero Retention:** Enterprise option
- **Location:** Customer choice (self-hosted)

### Cloud Platforms (Bedrock/Vertex/Azure)
- **Configurable:** Data handling varies by configuration
- **Zero Retention:** Available via API settings
- **Enterprise:** Custom agreements
- **Location:** Multiple regions

---

## Training Data Usage

| Tool | Uses Customer Code for Training | Opt-Out | Notes |
|------|--------------------------------|---------|-------|
| **GitHub Copilot** | ⚠️ Yes (public code) | ✅ Enterprise | Public repos only |
| **Cursor** | ❌ No | N/A | Claims no training use |
| **Windsurf** | ❌ No | N/A | Claims no training use |
| **OpenAI Codex** | ❌ No (API) | ✅ Default no training | Business terms |
| **Claude Code** | ❌ No | ✅ Default no training | Anthropic policy |
| **Gemini** | ⚠️ Possible | ✅ Enterprise controls | Google terms |
| **Kiro** | ❌ No | N/A | AWS doesn't train |
| **Tabnine** | ❌ No | ✅ Enterprise | Self-hosted = no sharing |
| **AWS Bedrock** | ❌ No | ✅ Configurable | AWS doesn't train |
| **Vertex AI** | ❌ No | ✅ Configurable | Google Cloud terms |
| **Azure Foundry** | ❌ No | ✅ Configurable | Microsoft terms |

---

## Security Certifications

| Tool | SOC 2 | ISO 27001 | GDPR | HIPAA |
|------|-------|-----------|------|-------|
| **GitHub Copilot** | ✅ Type II | ✅ | ✅ | ✅ BAA available |
| **Cursor** | ⚠️ In progress | ❌ | ✅ | ❌ |
| **Windsurf** | ⚠️ In progress | ❌ | ✅ | ❌ |
| **OpenAI Codex** | ✅ Type II | ✅ | ✅ | ✅ BAA available |
| **Claude Code** | ✅ Type II | ✅ | ✅ | ⚠️ In progress |
| **Gemini** | ✅ | ✅ | ✅ | ✅ BAA available |
| **Kiro** | ✅ | ✅ | ✅ | ✅ BAA available |
| **Tabnine** | ✅ Type II | ✅ | ✅ | ⚠️ Enterprise |
| **AWS Bedrock** | ✅ | ✅ | ✅ | ✅ BAA available |
| **Vertex AI** | ✅ | ✅ | ✅ | ✅ BAA available |
| **Azure Foundry** | ✅ | ✅ | ✅ | ✅ BAA available |

---

## Enterprise Controls

### Admin Features Available

| Feature | GitHub | Cursor | Windsurf | OpenAI | Claude | Gemini | Kiro | Tabnine |
|---------|--------|--------|----------|--------|--------|--------|------|---------|
| **SSO/SAML** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **Audit Logs** | ✅ | ✅ | ⚠️ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **Usage Analytics** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **Policy Controls** | ✅ | ✅ | ⚠️ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **IP Allowlisting** | ✅ | ❌ | ❌ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **Custom Models** | ❌ | ❌ | ❌ | ✅ | ✅ | ✅ | ❌ | ✅ |

---

## Recommendations by Use Case

### Maximum Privacy (Code Never Leaves)
- **Tabnine Enterprise** (self-hosted)
- **Local LLMs** (Ollama, etc.)

### Zero Data Retention
- **OpenAI Codex** (API with ZDR)
- **Claude Code** (API with ZDR)
- **AWS Bedrock** (configured)
- **Tabnine Enterprise**

### HIPAA Compliance
- **GitHub Copilot Enterprise**
- **OpenAI Enterprise**
- **AWS Bedrock** (with BAA)
- **Azure Foundry** (with BAA)

### GDPR Compliance
- All major tools claim compliance
- EU data residency options available
- DPA required for enterprise

### Government/Classified
- **AWS GovCloud** (Kiro, Bedrock)
- **Azure Government**
- **Self-hosted options**

---

## Key Questions to Ask Vendors

1. **Where is my data processed and stored?**
2. **Is my code used to train your models?**
3. **How long do you retain my code/prompts?**
4. **Can I opt-out of data retention?**
5. **What certifications do you have?**
6. **Can you sign a custom DPA?**
7. **Do you offer self-hosted options?**
8. **What audit rights do I have?**

---

*Last Updated: March 14, 2026*
