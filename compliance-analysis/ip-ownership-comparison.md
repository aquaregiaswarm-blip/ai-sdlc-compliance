# IP Ownership and Indemnification Comparison

## Overview

This document compares intellectual property ownership and indemnification provisions across AI coding tools.

---

## Code Ownership

### Who Owns AI-Generated Code?

| Tool | User Owns Output | Assignment to User | Notes |
|------|------------------|-------------------|-------|
| **GitHub Copilot** | ✅ Yes | ✅ Explicit | User retains all rights |
| **Cursor** | ✅ Yes | ✅ Explicit | User owns output |
| **Windsurf** | ✅ Yes | ✅ Explicit | User owns output |
| **OpenAI Codex** | ✅ Yes | ✅ Explicit | User retains all rights |
| **Claude Code** | ✅ Yes | ✅ Explicit | Anthropic assigns rights |
| **Gemini Code Assist** | ✅ Yes | ✅ Explicit | Google assigns rights |
| **Kiro (AWS)** | ✅ Yes | ✅ Explicit | AWS assigns rights |
| **Tabnine** | ✅ Yes | ✅ Explicit | User owns output |
| **AWS Bedrock** | ⚠️ Varies | ⚠️ By model | Check specific model terms |
| **Vertex AI** | ✅ Yes | ✅ Explicit | Google assigns rights |
| **Azure Foundry** | ✅ Yes | ✅ Explicit | Microsoft assigns rights |

**Key Point:** All major tools explicitly assign ownership of generated code to the user.

---

## Indemnification

### Copyright Indemnification

| Tool | Offers Indemnification | Scope | Limitations |
|------|----------------------|-------|-------------|
| **GitHub Copilot** | ⚠️ Limited | Enterprise only | Up to $10M |
| **Cursor** | ❌ No | N/A | User assumes risk |
| **Windsurf** | ❌ No | N/A | User assumes risk |
| **OpenAI Codex** | ✅ Yes | Business/Enterprise | Up to policy limits |
| **Claude Code** | ✅ Yes | Commercial | Up to policy limits |
| **Gemini** | ⚠️ Limited | Enterprise only | Case by case |
| **Kiro (AWS)** | ✅ Yes | Standard AWS | Up to AWS limits |
| **Tabnine** | ⚠️ Limited | Enterprise only | Custom agreements |
| **AWS Bedrock** | ⚠️ Varies | By model provider | Check model terms |
| **Vertex AI** | ⚠️ Limited | Enterprise | Google Cloud terms |
| **Azure Foundry** | ✅ Yes | Standard Microsoft | Up to Microsoft limits |

### What Indemnification Covers

**Typically Covered:**
- Third-party copyright claims
- Patent infringement claims
- Trade secret misappropriation

**Typically Excluded:**
- User's own infringing content
- Modifications to generated code
- Combination with other software
- Known infringement at time of use

---

## Open Source Compliance

### Training Data Transparency

| Tool | Discloses Training Data | Open Source Licenses | Filtering |
|------|------------------------|---------------------|-----------|
| **GitHub Copilot** | ⚠️ Partial | Claims fair use | Some filtering |
| **Cursor** | ❌ No | Not disclosed | Unknown |
| **Windsurf** | ❌ No | Not disclosed | Unknown |
| **OpenAI Codex** | ⚠️ Partial | Claims fair use | Some filtering |
| **Claude Code** | ⚠️ Partial | Claims fair use | Some filtering |
| **Gemini** | ⚠️ Partial | Claims fair use | Some filtering |
| **Kiro** | ⚠️ Partial | AWS + model provider | Varies |
| **Tabnine** | ✅ More transparent | Open source compliant | Yes - claims compliance |
| **AWS Bedrock** | ⚠️ By model | Varies by model | Varies |
| **Vertex AI** | ⚠️ Partial | Google + model provider | Varies |
| **Azure Foundry** | ⚠️ Partial | Microsoft + model provider | Varies |

### GPL and Copyleft Concerns

**The Problem:**
- AI models trained on GPL code may generate GPL-licensed code
- Users may unknowingly incorporate GPL code into proprietary projects
- Legal risk of license violation

**Vendor Positions:**
- Most claim "fair use" for training
- Few offer copyleft filtering
- No vendor guarantees GPL-free output

**Mitigation Strategies:**
1. Code scanning tools (Snyk, FOSSA, Black Duck)
2. License compliance checks in CI/CD
3. Legal review of AI-generated code
4. Avoiding AI for security-critical code

---

## Warranty Disclaimers

### Standard Disclaimer Language

All AI coding tools disclaim warranties:

> "AS IS" and "AS AVAILABLE" basis  
> No warranties of merchantability  
> No warranties of fitness for purpose  
> No guarantee of accuracy  
> No guarantee of non-infringement

### What This Means

- Vendors don't guarantee code works
- Vendors don't guarantee code is secure
- Vendors don't guarantee code is original
- User bears all risk of use

### Enterprise Protections

Some enterprise agreements include:
- Service level agreements (SLAs)
- Uptime guarantees
- Support commitments
- Custom warranties (negotiated)

---

## Liability Limitations

### Standard Liability Caps

| Tool | Liability Cap | Exceptions |
|------|--------------|------------|
| **GitHub Copilot** | Fees paid in 12 months | IP indemnification, gross negligence |
| **Cursor** | Fees paid in 12 months | Gross negligence, willful misconduct |
| **Windsurf** | Fees paid in 12 months | Gross negligence, willful misconduct |
| **OpenAI** | Fees paid in 12 months | IP indemnification, gross negligence |
| **Claude** | Fees paid in 12 months | IP indemnification, gross negligence |
| **Gemini** | Fees paid in 12 months | IP indemnification, gross negligence |
| **AWS** | Standard AWS terms | IP indemnification, gross negligence |
| **Tabnine** | Fees paid in 12 months | IP indemnification (enterprise) |
| **Azure** | Standard Microsoft terms | IP indemnification, gross negligence |

### What This Means

- Maximum recovery is typically 12 months of fees
- IP indemnification often has separate higher limits
- Gross negligence/willful misconduct not capped
- Consequential damages excluded

---

## Recommendations

### For Legal Protection

1. **Choose tools with indemnification:**
   - OpenAI Codex (Business+)
   - Claude Code (Commercial)
   - AWS/Azure (Enterprise)
   - GitHub Copilot (Enterprise)

2. **Implement code scanning:**
   - Snyk, FOSSA, or Black Duck
   - License compliance checks
   - Security vulnerability scanning

3. **Establish AI usage policies:**
   - When AI can be used
   - Required review processes
   - Prohibited use cases
   - Documentation requirements

4. **Negotiate enterprise agreements:**
   - Custom indemnification
   - Higher liability caps
   - Specific warranties
   - Audit rights

### For Risk Mitigation

1. **Don't use AI for:**
   - Security-critical code
   - Cryptographic implementations
   - Regulatory compliance code
   - Patent-sensitive innovations

2. **Always review AI-generated code:**
   - Security review
   - License compliance check
   - Code quality review
   - Architecture fit

3. **Document AI usage:**
   - What was AI-generated
   - What was reviewed
   - Who reviewed it
   - When it was reviewed

---

## Key Legal Questions

1. **Does the vendor indemnify for copyright infringement?**
2. **What is the indemnification cap?**
3. **Does the vendor disclose training data?**
4. **How does the vendor handle GPL/copyleft?**
5. **What warranties are provided?**
6. **What is the liability cap?**
7. **Can we negotiate custom terms?**

---

*Last Updated: March 14, 2026*

**Disclaimer:** This is not legal advice. Consult qualified legal counsel for specific guidance.
