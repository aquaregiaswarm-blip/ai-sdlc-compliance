# AI Governance Board Review
## AI-Powered Software Development Tools

**Prepared for:** Organization Controls Compliance Review  
**Date:** March 14, 2026  
**Prepared by:** Aqua Regia 🜆

---

## Executive Summary

This document provides a comprehensive governance review of AI-powered software development tools for enterprise adoption. It covers 12 major AI coding assistants and cloud AI platforms, analyzing compliance implications across data handling, intellectual property, security, and regulatory frameworks.

---

## Tools Under Review

### Individual AI Coding Assistants
1. **GitHub Copilot** (GitHub/Microsoft)
2. **Cursor** (Anysphere)
3. **Windsurf** (Codeium)
4. **OpenAI Codex** (OpenAI)
5. **Claude Code** (Anthropic)
6. **Gemini Code Assist** (Google)
7. **Kiro** (AWS)
8. **Tabnine** (Tabnine)

### Cloud AI Platforms
9. **AWS Bedrock - Anthropic Claude**
10. **AWS Bedrock - OpenAI Models**
11. **Google Vertex AI**
12. **Microsoft Azure AI Foundry**

---

## 1. Enterprise Costing Models

### Individual AI Coding Assistants

| Tool | Individual | Team | Enterprise | Billing Model |
|------|-----------|------|------------|---------------|
| **GitHub Copilot** | $10/mo | $19/mo/user | $39/mo/user | Per user/month |
| **Cursor** | Free tier | $20/mo/user | Custom | Per user/month |
| **Windsurf** | Free tier | $15/mo/user | Custom | Per user/month |
| **OpenAI Codex** | API usage | API usage | Custom contract | Per token/request |
| **Claude Code** | API usage | API usage | Custom contract | Per token/request |
| **Gemini Code Assist** | Free tier | $19/mo/user | Custom | Per user/month |
| **Kiro** | Included with AWS | AWS usage | Enterprise support | AWS billing |
| **Tabnine** | $12/mo | $20/mo/user | Custom | Per user/month |

### Cloud AI Platforms

| Platform | On-Demand | Provisioned | Enterprise | Notes |
|----------|-----------|-------------|------------|-------|
| **AWS Bedrock** | Per token | Custom | EDP discounts | Volume discounts |
| **Vertex AI** | Per token | Committed use | Custom | Sustained use discounts |
| **Azure Foundry** | Per token | Reserved | EA discounts | Azure commitment |

### Hidden Costs to Consider
- **Integration costs:** IDE plugins, CI/CD pipelines
- **Training costs:** Developer onboarding
- **Compliance costs:** Legal review, DPA negotiations
- **Support costs:** Premium support tiers
- **Data egress:** Cloud platform fees

---

## 2. Available Models

### Code Generation Models

| Tool | Primary Model | Alternative Models | Context Window |
|------|--------------|-------------------|----------------|
| **GitHub Copilot** | GPT-4 (Codex) | GPT-3.5 | 8K-32K tokens |
| **Cursor** | GPT-4, Claude | Custom routing | 200K (Claude) |
| **Windsurf** | GPT-4, Claude | Codeium models | 200K (Claude) |
| **OpenAI Codex** | Codex (latest) | GPT-4, GPT-3.5 | 128K tokens |
| **Claude Code** | Claude 3.5 Sonnet | Claude 3 Opus, Haiku | 200K tokens |
| **Gemini Code Assist** | Gemini 1.5 Pro | Gemini 1.5 Flash | 1M tokens |
| **Kiro** | Amazon models | Bedrock integration | Varies |
| **Tabnine** | Proprietary | Open source models | 4K-8K tokens |

### Cloud Platform Models

| Platform | Models Available | Fine-Tuning | Custom Models |
|----------|-----------------|-------------|---------------|
| **AWS Bedrock** | Claude, GPT, Llama, Mistral, Jurassic | ✅ Yes | ✅ Via SageMaker |
| **Vertex AI** | Gemini, PaLM, Codey, Imagen | ✅ Yes | ✅ Model Garden |
| **Azure Foundry** | GPT-4, Codex, Llama, Mistral | ✅ Yes | ✅ Azure ML |

### Model Selection Considerations
- **Performance:** Code quality, accuracy
- **Latency:** Response time requirements
- **Cost:** Token pricing varies significantly
- **Capability:** Language support, context understanding
- **Compliance:** Model training data transparency

---

## 3. Data Residency

### Where Code/Data Is Processed

| Tool | Primary Region | EU Option | Asia-Pacific | On-Premise |
|------|---------------|-----------|--------------|------------|
| **GitHub Copilot** | US | ✅ EU data boundary | ✅ | ❌ |
| **Cursor** | US | ⚠️ Limited | ⚠️ Limited | ❌ |
| **Windsurf** | US | ⚠️ Limited | ⚠️ Limited | ✅ Enterprise |
| **OpenAI Codex** | US | ✅ EU residency | ✅ | ❌ |
| **Claude Code** | US | ⚠️ Coming soon | ⚠️ Coming soon | ❌ |
| **Gemini Code Assist** | US | ✅ EU options | ✅ | ❌ |
| **Kiro** | AWS regions | ✅ All regions | ✅ | ✅ AWS Outposts |
| **Tabnine** | US/EU | ✅ EU hosting | ✅ | ✅ Self-hosted |

### Cloud Platforms

| Platform | Global Regions | Data Residency Controls | Sovereign Cloud |
|----------|---------------|------------------------|-----------------|
| **AWS Bedrock** | 30+ regions | ✅ Per-request | ✅ AWS GovCloud |
| **Vertex AI** | 35+ regions | ✅ Location-specific | ✅ Assured Workloads |
| **Azure Foundry** | 60+ regions | ✅ Region selection | ✅ Azure Government |

### Data Residency Requirements
- **GDPR:** EU data must stay in EU
- **Schrems II:** US-EU data transfer restrictions
- **National laws:** China, Russia data localization
- **Industry:** Healthcare, finance specific requirements

---

## 4. Tenant Data Isolation Options

### Code/Data Retention Controls

| Tool | Zero Data Retention | Training Opt-Out | Custom Retention | Audit Logs |
|------|--------------------|------------------|------------------|------------|
| **GitHub Copilot** | ❌ No | ✅ Enterprise | ❌ Fixed | ✅ Enterprise |
| **Cursor** | ❌ No | ✅ Enterprise | ⚠️ Limited | ✅ Enterprise |
| **Windsurf** | ❌ No | ✅ Enterprise | ⚠️ Limited | ✅ Enterprise |
| **OpenAI Codex** | ✅ API option | ✅ Default | ✅ Configurable | ✅ Business |
| **Claude Code** | ✅ API option | ✅ Default | ✅ Configurable | ✅ Commercial |
| **Gemini Code Assist** | ❌ No | ✅ Enterprise | ⚠️ Limited | ✅ Enterprise |
| **Kiro** | ✅ Available | ✅ Default | ✅ AWS controls | ✅ CloudTrail |
| **Tabnine** | ✅ Enterprise | ✅ Enterprise | ✅ Configurable | ✅ Enterprise |

### Tenant Isolation Features

| Feature | Description | Availability |
|---------|-------------|--------------|
| **VPC/VNet Integration** | Private network connectivity | AWS, Azure, GCP |
| **Private Endpoints** | No public internet exposure | Enterprise tiers |
| **Encryption at Rest** | Customer-managed keys (CMK) | Enterprise tiers |
| **Encryption in Transit** | TLS 1.3, mTLS | All tiers |
| **Data Loss Prevention** | Content filtering, scanning | Enterprise add-on |

### Keeping Data In Your Tenant

**Best Practices:**
1. **Self-hosted options:** Tabnine Enterprise, Windsurf Enterprise
2. **Private cloud:** AWS VPC, Azure VNet, GCP VPC
3. **Zero data retention:** Configure API options (OpenAI, Anthropic)
4. **Opt-out of training:** Explicitly disable in settings
5. **Audit logging:** Enable comprehensive logging
6. **Network controls:** IP allowlisting, VPN requirements

---

## 5. Hyperscaler Availability

### AWS (Amazon Web Services)

**Native Services:**
- **Kiro** - AWS-native IDE integration
- **Amazon Q Developer** - AWS's own AI assistant
- **AWS Bedrock** - Foundation model API

**Available Through Bedrock:**
- Anthropic Claude (all versions)
- OpenAI GPT (limited)
- Meta Llama
- Mistral AI
- Amazon Titan

**Integration:**
- IAM authentication
- CloudTrail logging
- KMS encryption
- VPC endpoints

### Google Cloud Platform

**Native Services:**
- **Gemini Code Assist** - Native GCP integration
- **Vertex AI** - Model hosting and API
- **Duet AI** (deprecated, merged into Gemini)

**Available Through Vertex AI:**
- Google Gemini (all versions)
- PaLM 2
- Codey
- Third-party models

**Integration:**
- Cloud IAM
- Cloud Audit Logs
- CMEK encryption
- VPC Service Controls

### Microsoft Azure

**Native Services:**
- **GitHub Copilot** - Microsoft-owned
- **Azure AI Foundry** - Model hosting platform
- **GitHub Copilot for Azure** - Azure-specific

**Available Through Azure Foundry:**
- OpenAI GPT (exclusive partnership)
- Llama
- Mistral
- Phi

**Integration:**
- Azure AD authentication
- Azure Monitor logging
- Customer-managed keys
- Private Link

### Multi-Cloud Strategy

| Approach | Pros | Cons |
|----------|------|------|
| **Single cloud** | Simplified management, better discounts | Vendor lock-in, limited redundancy |
| **Multi-cloud** | Best-of-breed, redundancy, negotiation leverage | Complexity, cost, integration challenges |
| **Cloud-agnostic tools** | Flexibility, portability | May lack deep integration |

---

## 6. Compliance Intent Alignment

### NIST AI Risk Management Framework

| Function | Tool Capabilities | Gap Analysis |
|----------|------------------|--------------|
| **Govern** | Admin controls, policies | Limited AI-specific governance |
| **Map** | Usage analytics, auditing | Need custom risk mapping |
| **Measure** | Performance metrics, bias testing | Limited automated measurement |
| **Manage** | Access controls, monitoring | Manual risk management |

### ISO/IEC 42001 (AI Management Systems)

| Requirement | Compliance Status | Action Required |
|-------------|------------------|-----------------|
| **Context of organization** | Partial | Define AI scope |
| **Leadership** | N/A | Internal governance |
| **Planning** | Partial | Risk assessment |
| **Support** | Varies by tool | Resource allocation |
| **Operation** | Partial | Process documentation |
| **Performance evaluation** | Limited | Monitoring setup |
| **Improvement** | Limited | Continuous review |

### EU AI Act Alignment

| Risk Level | Applicability | Requirements |
|------------|--------------|--------------|
| **Unacceptable risk** | Not applicable | AI coding assistants not prohibited |
| **High risk** | Possible | If used in critical systems |
| **Limited risk** | Likely | Transparency obligations |
| **Minimal risk** | Possible | Basic requirements |

### Industry-Specific Compliance

| Industry | Regulations | Tool Considerations |
|----------|------------|---------------------|
| **Healthcare** | HIPAA, FDA | BAA required, validation needed |
| **Financial Services** | SOX, GLBA, PCI-DSS | Audit trails, segregation |
| **Government** | FedRAMP, StateRAMP | Authorized cloud services |
| **Defense** | CMMC, ITAR | Air-gapped options |

---

## 7. Key Governance Considerations

### Data Governance

**Questions for the Board:**
1. What code leaves our environment?
2. Where is it processed and stored?
3. Is it used to train AI models?
4. How long is it retained?
5. Can we delete it on request?

**Recommended Controls:**
- Data classification policy
- AI tool usage policy
- Data retention schedules
- Deletion procedures
- Audit mechanisms

### Intellectual Property

**Questions for the Board:**
1. Who owns AI-generated code?
2. What indemnification do vendors provide?
3. How do we handle open source compliance?
4. What patent risks exist?
5. How do we protect trade secrets?

**Recommended Controls:**
- IP ownership verification
- Vendor indemnification review
- Open source scanning (Snyk, FOSSA)
- Code review requirements
- Documentation standards

### Security Governance

**Questions for the Board:**
1. What access controls are in place?
2. How is data encrypted?
3. What audit logs are available?
4. How do we detect misuse?
5. What is our incident response plan?

**Recommended Controls:**
- SSO/SAML enforcement
- MFA requirements
- Network segmentation
- DLP implementation
- Security monitoring

### Vendor Management

**Questions for the Board:**
1. What is our vendor risk assessment process?
2. Do vendors have required certifications?
3. What are our exit strategies?
4. How do we ensure business continuity?
5. What contractual protections do we have?

**Recommended Controls:**
- Vendor risk assessments
- Certification verification (SOC 2, ISO 27001)
- Contract review process
- Exit planning
- Regular vendor reviews

---

## 8. Recommendations

### Immediate Actions

1. **Legal Review**
   - Review ToS, DPA, Privacy Policy for selected tools
   - Negotiate enterprise agreements
   - Obtain legal sign-off

2. **Policy Development**
   - Create AI usage policy
   - Define approved/prohibited use cases
   - Establish review requirements

3. **Pilot Program**
   - Start with low-risk projects
   - Measure productivity gains
   - Assess compliance impact

4. **Training**
   - Developer training on AI tools
   - Security awareness
   - Compliance requirements

### Short-Term (3-6 months)

1. **Implementation**
   - Deploy to development teams
   - Configure enterprise controls
   - Enable audit logging

2. **Monitoring**
   - Usage analytics
   - Security monitoring
   - Compliance audits

3. **Optimization**
   - Cost optimization
   - Performance tuning
   - Process refinement

### Long-Term (6-12 months)

1. **Expansion**
   - Broader deployment
   - Additional use cases
   - Advanced features

2. **Governance Maturity**
   - AI governance committee
   - Regular risk assessments
   - Continuous improvement

3. **Strategic Planning**
   - Multi-year roadmap
   - Vendor relationship management
   - Emerging technology evaluation

---

## 9. Risk Assessment Summary

| Risk Category | Level | Mitigation |
|--------------|-------|------------|
| **Data privacy** | Medium | DPA, encryption, opt-out |
| **IP infringement** | Medium | Indemnification, scanning |
| **Security** | Low-Medium | Enterprise controls, monitoring |
| **Vendor lock-in** | Medium | Multi-vendor strategy |
| **Regulatory** | Medium | Compliance review, documentation |
| **Operational** | Low | Training, support |

---

## 10. Next Steps

1. **Board Decision:** Approve AI tool adoption framework
2. **Legal:** Complete vendor contract review
3. **Security:** Finalize security assessment
4. **IT:** Prepare deployment plan
5. **Compliance:** Establish ongoing monitoring

---

*Document prepared by Aqua Regia 🜆*  
*For questions or updates, contact compliance team*
