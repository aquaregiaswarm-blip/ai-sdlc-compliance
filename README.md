# AI SDLC Compliance Repository

> Legal Documents and Compliance Analysis for AI-Powered Software Development Tools

---

🜆 *"Dissolving compliance complexity like royal water dissolves noble metals"* — Aqua Regia

---

## Overview

This repository contains Terms of Service (ToS), Data Processing Agreements (DPA), and Privacy Policies for AI-powered software development tools. These documents are essential for:

- **Legal Compliance:** Understanding obligations when using AI coding assistants
- **Enterprise Procurement:** Evaluating AI tools for organizational use
- **Risk Assessment:** Identifying data handling and security implications
- **Policy Development:** Creating internal AI usage policies

---

## Repository Structure

```
ai-sdlc-compliance/
├── README.md                           # This file
├── legal-documents/                    # Raw legal documents
│   ├── github-copilot/
│   ├── cursor/
│   ├── windsurf/
│   ├── openai-codex/
│   ├── claude-code/
│   ├── gemini-code-assist/
│   ├── kiro-aws/
│   ├── tabnine/
│   ├── aws-bedrock-anthropic/
│   ├── aws-bedrock-openai/
│   ├── vertex-ai/
│   └── azure-foundry/
├── compliance-analysis/                # Side-by-side comparisons
│   ├── data-handling-comparison.md
│   ├── ip-ownership-comparison.md
│   ├── security-comparison.md
│   └── enterprise-features-comparison.md
└── templates/                          # Internal policy templates
    ├── ai-tool-usage-policy-template.md
    └── vendor-evaluation-checklist.md
```

---

## Tools Covered

### Individual AI Coding Assistants

| Tool | Provider | Type | Enterprise Ready |
|------|----------|------|------------------|
| GitHub Copilot | GitHub/Microsoft | Code completion | ✅ |
| Cursor | Anysphere | IDE + AI | ✅ |
| Windsurf | Codeium | IDE + AI | ✅ |
| OpenAI Codex | OpenAI | CLI + API | ✅ |
| Claude Code | Anthropic | CLI | ✅ |
| Gemini Code Assist | Google | IDE + Cloud | ✅ |
| Kiro | AWS | IDE + Cloud | ✅ |
| Tabnine | Tabnine | Code completion | ✅ |

### Cloud AI Platforms

| Platform | Provider | Models Available | Enterprise Ready |
|----------|----------|------------------|------------------|
| AWS Bedrock | Amazon | Claude, GPT, Llama, etc. | ✅ |
| Vertex AI | Google | Gemini, PaLM, etc. | ✅ |
| Azure Foundry | Microsoft | GPT, Codex, etc. | ✅ |

---

## Key Compliance Areas

### 1. Data Processing & Privacy
- What code/data is sent to AI providers?
- How is data retained and stored?
- Is data used for model training?
- GDPR/CCPA compliance mechanisms

### 2. Intellectual Property
- Who owns AI-generated code?
- Indemnification for copyright claims
- Open source license compliance
- Training data transparency

### 3. Security & Confidentiality
- SOC 2 compliance
- Encryption standards
- Data residency options
- Network security

### 4. Enterprise Features
- SSO/SAML support
- Audit logging
- Admin controls
- Usage analytics

---

## Quick Reference

### Data Handling Summary

| Tool | Code Sent to Cloud | Training Opt-Out | Zero Data Retention | Enterprise Controls |
|------|-------------------|------------------|---------------------|---------------------|
| GitHub Copilot | Yes | ✅ | ❌ | ✅ |
| Cursor | Yes | ✅ | ❌ | ✅ |
| Windsurf | Yes | ✅ | ❌ | ✅ |
| OpenAI Codex | Yes | ✅ | ✅ (API) | ✅ |
| Claude Code | Yes | ✅ | ✅ (API) | ✅ |
| Gemini Code Assist | Yes | ✅ | ❌ | ✅ |
| Kiro (AWS) | Yes | ✅ | ✅ | ✅ |
| Tabnine | Optional | ✅ | ✅ (Enterprise) | ✅ |
| AWS Bedrock | Yes | ✅ | ✅ | ✅ |
| Vertex AI | Yes | ✅ | ✅ | ✅ |
| Azure Foundry | Yes | ✅ | ✅ | ✅ |

### IP Ownership Summary

| Tool | User Owns Output | Indemnification | Open Source Compliance |
|------|-----------------|-----------------|----------------------|
| GitHub Copilot | ✅ | Limited | Partial |
| Cursor | ✅ | Limited | Partial |
| Windsurf | ✅ | Limited | Partial |
| OpenAI Codex | ✅ | ✅ | Partial |
| Claude Code | ✅ | ✅ | Partial |
| Gemini Code Assist | ✅ | Limited | Partial |
| Kiro (AWS) | ✅ | ✅ | Partial |
| Tabnine | ✅ | Limited | ✅ |
| AWS Bedrock | Varies by model | Varies | Partial |
| Vertex AI | ✅ | Limited | Partial |
| Azure Foundry | ✅ | ✅ | Partial |

---

## Usage Guidelines

### For Legal Teams
1. Review ToS for each tool in `legal-documents/`
2. Compare DPAs for data handling requirements
3. Check Privacy Policies for GDPR/CCPA compliance
4. Use comparison matrices in `compliance-analysis/`

### For Engineering Teams
1. Understand what code leaves your environment
2. Know your opt-out rights for training data
3. Review security requirements
4. Follow internal AI usage policies

### For Procurement
1. Evaluate enterprise features
2. Compare pricing models
3. Assess vendor security posture
4. Negotiate DPA amendments if needed

---

## Important Disclaimers

⚠️ **Legal Notice:**
- This repository is for informational purposes only
- Documents are downloaded from public sources
- Always verify current versions with vendors
- Consult legal counsel for compliance decisions

⚠️ **Accuracy:**
- Documents may become outdated
- Check vendor websites for latest versions
- Terms change frequently
- Last updated dates noted in each file

⚠️ **Not Legal Advice:**
- This is not legal advice
- Not a substitute for professional counsel
- Compliance requirements vary by jurisdiction
- Organization-specific factors apply

---

## Contributing

To add new tools or update documents:
1. Download latest ToS/DPA/Privacy Policy
2. Place in appropriate `legal-documents/` subdirectory
3. Update comparison matrices
4. Submit PR with source URLs and dates

---

## Resources

### Vendor Documentation
- Links to official documentation
- API references
- Enterprise guides

### Regulatory Resources
- NIST AI Risk Management Framework
- ISO/IEC 42001 (AI Management Systems)
- EU AI Act compliance guides
- State AI legislation references

---

## License

This repository is provided for educational and compliance purposes. Legal documents remain property of their respective vendors.

---

*Repository maintained by Aqua Regia 🜆*  
*For Essex Technology Group compliance initiatives*
