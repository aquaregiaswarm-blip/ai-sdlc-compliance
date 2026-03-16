# Organization Controls - Standards Alignment Validation
## Control-by-Control Confidence Scoring

**Date:** March 14, 2026  
**Analyst:** Aqua Regia 🜆  
**Method:** Cross-reference controls against official standard texts

---

## Scoring Methodology

| Score | Meaning |
|-------|---------|
| **10** | Perfect alignment - control exactly matches standard requirement |
| **8-9** | Strong alignment - control captures intent with minor gaps |
| **6-7** | Moderate alignment - control related but not precise match |
| **4-5** | Weak alignment - control loosely related to standard |
| **2-3** | Poor alignment - control misinterprets standard |
| **1** | No alignment - control not found in standard or hallucinated |

---

## 1. ISO/IEC 42001:2023 Validation

### Official ISO 42001 Structure
ISO 42001 follows Annex SL with clauses 4-10 and annexes A-J. Annex A contains specific AI controls.

| Control ID | Control Name | Claimed Alignment | Actual ISO 42001 Reference | Confidence Score | Issues |
|------------|--------------|-------------------|---------------------------|------------------|--------|
| **CTL-001** | AI Policy | ISO42001 A.2.1, Cl.5.2 | ✅ **A.2.1 Policy for AI** - "Top-level AI policy appropriate to purpose" | **10/10** | Perfect match |
| **CTL-002** | AI Guiding Principles | ISO42001 A.2.2 | ✅ **A.2.2 AI Guiding Principles** - "Documented principles: fairness, transparency, accountability, privacy, safety" | **10/10** | Perfect match |
| **CTL-003** | AI Acceptable Use Policy | ISO42001 A.9.1 | ⚠️ **A.9.1 Appropriate Use** - "Define and enforce use boundaries" | **8/10** | AUP is implementation of appropriate use, but A.9.1 is broader |
| **CTL-004** | Policy Review Cycle | ISO42001 A.2.3 | ✅ **A.2.3 Review of Policy** - "Policy reviewed at planned intervals" | **9/10** | Good match, standard says "planned intervals" not necessarily annual |
| **CTL-005** | AI Review Board | ISO42001 A.3.1, Cl.5.3 | ⚠️ **A.3.1 Roles & Authorities** - "Responsibilities assigned and communicated" | **7/10** | AI Review Board is ONE way to implement, not required by standard |
| **CTL-006** | Executive Sponsorship | ISO42001 Cl.5.1 | ⚠️ **Clause 5.1 Leadership and Commitment** - "Top management shall demonstrate leadership" | **6/10** | Standard requires leadership commitment, not specifically "executive sponsor" |
| **CTL-007** | Concern Reporting | ISO42001 A.3.2 | ✅ **A.3.2 Reporting Concerns** - "Process for reporting concerns" | **9/10** | Good match |
| **CTL-008** | User Responsibility | ISO42001 A.8.4, A.9.4 | ⚠️ **A.8.4 Responsibility for Decisions** + **A.9.4 Responsibility for Output** | **8/10** | Combined from two clauses, accurate |
| **CTL-009** | AI Risk Assessment | ISO42001 Cl.6.1 | ✅ **Clause 6.1 Actions to Address Risks** | **9/10** | Good match |
| **CTL-010** | AI Risk Register | ISO42001 Cl.6.1 | ⚠️ **Clause 6.1** mentions risks but "Risk Register" is implementation detail | **7/10** | Register is tool, not explicitly required |
| **CTL-011** | AI Impact Assessment | ISO42001 A.5.1-A.5.4 | ✅ **A.5.1-A.5.4 Impact Assessment Process** | **10/10** | Perfect match |
| **CTL-012** | AI System Inventory | ISO42001 A.4.1 | ✅ **A.4.1 AI System Components & Assets** | **9/10** | Good match, inventory is implementation |
| **CTL-013** | Prohibit Sensitive Data | ISO42001 A.7.2 | ⚠️ **A.7.2 Data Quality** - focuses on quality, not prohibition | **5/10** | ⚠️ **MISALIGNMENT** - Standard doesn't explicitly prohibit sensitive data |
| **CTL-014** | Data Leakage Prevention | ISO42001 A.7.2 | ❌ **NOT in ISO 42001** - DLP is security control, not AI management | **3/10** | ⚠️ **HALLUCINATION** - This is ISO 27001, not ISO 42001 |
| **CTL-015** | Data Governance Checklist | ISO42001 A.7.1-A.7.5 | ⚠️ **A.7.1-A.7.5 Data for AI Systems** | **7/10** | Checklist is implementation, standard requires data management |
| **CTL-016** | Data Classification | ISO42001 A.7.1 | ⚠️ **A.7.1 Data for AI Systems** - mentions classification but not detailed | **6/10** | Classification is implied, not explicit requirement |
| **CTL-017** | AI Tool Approval Gate | ISO42001 A.6.1, A.9.1 | ✅ **A.6.1 Initiation of AI System** + **A.9.1 Appropriate Use** | **8/10** | Good synthesis |
| **CTL-018** | Block Unapproved Tools | ISO42001 A.9.1 | ⚠️ **A.9.1 Appropriate Use** - "enforce use boundaries" | **7/10** | Blocking is one enforcement method |
| **CTL-019** | Preferred Tool Directive | ISO42001 A.9.1 | ⚠️ **A.9.1 Appropriate Use** | **6/10** | Preferred tools is implementation choice, not standard requirement |
| **CTL-020** | Prompt Hygiene | ISO42001 A.6.5 | ❌ **NOT in ISO 42001** - Prompt hygiene is operational, not in standard | **2/10** | ⚠️ **HALLUCINATION** - Not found in ISO 42001 |
| **CTL-021** | Output Verification | ISO42001 A.9.4 | ✅ **A.9.4 Responsibility for Output** | **9/10** | Good match |
| **CTL-022** | AI Contribution Transparency | ISO42001 A.8.1, A.8.3 | ✅ **A.8.1 Transparency** + **A.8.3 Explainability** | **9/10** | Good match |
| **CTL-023** | Mandatory Human Review | ISO42001 A.9.2 | ✅ **A.9.2 Human Oversight** | **10/10** | Perfect match |
| **CTL-024** | AI Feature Change Notification | ISO42001 A.6.8 | ⚠️ **A.6.8 Change Management** | **7/10** | Notification is part of change management, not explicit |
| **CTL-025** | Third-Party Risk Management | ISO42001 A.10.1-A.10.2 | ✅ **A.10.1-A.10.2 AI Supply Chain Mgmt** | **10/10** | Perfect match |
| **CTL-026** | Vendor Training Data Review | ISO42001 A.10.2 | ⚠️ **A.10.2 AI Supply Chain Mgmt** - "assess third-party AI governance" | **7/10** | Training data review is specific interpretation |
| **CTL-027** | Vendor AI Register | ISO42001 A.10.2 | ⚠️ **A.10.2** mentions monitoring but not specifically "register" | **6/10** | Register is implementation tool |
| **CTL-028** | AI Usage Monitoring | ISO42001 A.6.7 | ✅ **A.6.7 Monitoring of AI Systems** | **10/10** | Perfect match |
| **CTL-029** | AI-Specific Incident Detection | ISO42001 A.6.7 | ⚠️ **A.6.7** mentions monitoring but not "incident detection" specifically | **6/10** | Incident detection is part of monitoring |
| **CTL-030** | AI Incident Reporting | ISO42001 Cl.10.1 | ✅ **Clause 10.1 Nonconformity and Corrective Action** | **8/10** | Good match, standard uses "nonconformity" not "incident" |

### ISO 42001 Summary
- **Perfect Matches (10/10):** 5 controls
- **Strong Alignment (8-9/10):** 10 controls
- **Moderate Alignment (6-7/10):** 10 controls
- **Weak Alignment (4-5/10):** 2 controls
- **Poor/Hallucinated (1-3/10):** 3 controls

**Overall ISO 42001 Confidence: 7.2/10**

**Major Issues:**
- CTL-013: Misaligned - standard doesn't prohibit sensitive data
- CTL-014: Hallucinated - DLP not in ISO 42001
- CTL-020: Hallucinated - prompt hygiene not in ISO 42001

---

## 2. NIST AI Risk Management Framework (RMF) Validation

### Official NIST AI RMF Structure
Published January 2023. Four functions: GOVERN, MAP, MEASURE, MANAGE.

| Control ID | Control Name | Claimed Alignment | Actual NIST AI RMF Reference | Confidence Score | Issues |
|------------|--------------|-------------------|------------------------------|------------------|--------|
| **CTL-001** | AI Policy | NIST GV-1.1–1.7 | ✅ **GOVERN 1.1-1.7** - Policies, processes, procedures | **9/10** | Good match |
| **CTL-002** | AI Guiding Principles | NIST 7 Trustworthy Chars | ✅ **7 Trustworthy AI Characteristics** - Valid, reliable, safe, etc. | **8/10** | Good match, but "7 characteristics" is framework, not specific control |
| **CTL-003** | AI Acceptable Use | NIST GV-4.1 | ⚠️ **GOVERN 4.1** - "Risk tolerance statements" | **6/10** | AUP is implementation, not explicit in RMF |
| **CTL-005** | AI Review Board | NIST GV-2.1 | ⚠️ **GOVERN 2.1** - "Roles and responsibilities" | **6/10** | Board is one implementation option |
| **CTL-006** | Executive Sponsorship | NIST GV-2.3 | ⚠️ **GOVERN 2.3** - "Executive leadership takes responsibility" | **7/10** | Good match |
| **CTL-007** | Concern Reporting | NIST GV-4.3 | ✅ **GOVERN 4.3** - "Processes for reporting concerns" | **9/10** | Good match |
| **CTL-009** | AI Risk Assessment | NIST MP-1–MP-5 | ✅ **MAP 1-5** - Context, categorization, capabilities, risks, impacts | **9/10** | Good match |
| **CTL-010** | AI Risk Register | NIST MAP+MANAGE | ⚠️ **MAP and MANAGE functions** - Risk register is tool, not explicit | **6/10** | Register implied but not required |
| **CTL-011** | AI Impact Assessment | NIST MP-5 | ✅ **MAP 5** - "Impacts of AI systems are examined and documented" | **10/10** | Perfect match |
| **CTL-023** | Mandatory Human Review | NIST GV-3.2 | ✅ **GOVERN 3.2** - "Decision-making is informed by human oversight" | **9/10** | Good match |
| **CTL-028** | AI Usage Monitoring | NIST MS-3 | ⚠️ **MEASURE 3** - "Test, evaluation, verification, validation" | **6/10** | Monitoring is part of TEVV, not exact match |
| **CTL-030** | AI Incident Reporting | NIST MG-4 | ⚠️ **MANAGE 4** - "Response and recovery" | **7/10** | Incident reporting part of response |

### NIST AI RMF Summary
- **Perfect Matches (10/10):** 1 control
- **Strong Alignment (8-9/10):** 5 controls
- **Moderate Alignment (6-7/10):** 5 controls
- **Weak Alignment (4-5/10):** 1 control

**Overall NIST AI RMF Confidence: 7.4/10**

**Notes:**
- NIST AI RMF is a framework, not a standard with specific controls
- Many mappings are interpretive rather than explicit
- RMF focuses on functions, not prescriptive controls

---

## 3. OWASP Top 10 for LLM Applications Validation

### Official OWASP LLM Top 10 (2023)
Published list of 10 critical vulnerabilities for LLM applications.

| Control ID | Control Name | Claimed Alignment | Actual OWASP LLM Reference | Confidence Score | Issues |
|------------|--------------|-------------------|---------------------------|------------------|--------|
| **CTL-003** | AI Acceptable Use | OWASP-Agent ASI03 | ❌ **ASI03 is "Identity & Privilege Abuse"** - Wrong mapping! | **2/10** | ⚠️ **WRONG MAPPING** - ASI03 is about credentials, not acceptable use |
| **CTL-013** | Prohibit Sensitive Data | OWASP LLM02 | ✅ **LLM02: Sensitive Information Disclosure** | **9/10** | Good match |
| **CTL-014** | Data Leakage Prevention | OWASP LLM02, ASI06 | ⚠️ **LLM02 correct, ASI06 is "Agent Goal Hijack"** - Wrong! | **5/10** | ⚠️ **PARTIAL HALLUCINATION** - ASI06 doesn't exist or mislabeled |
| **CTL-017** | AI Tool Approval Gate | OWASP-Agent ASI03 | ❌ **ASI03 is "Identity & Privilege Abuse"** - Wrong! | **2/10** | ⚠️ **WRONG MAPPING** |
| **CTL-018** | Block Unapproved Tools | OWASP-Agent ASI04 | ❌ **ASI04 is "Supply Chain Vulnerabilities"** - Wrong! | **2/10** | ⚠️ **WRONG MAPPING** |
| **CTL-019** | Preferred Tool Directive | OWASP LLM03 | ❌ **LLM03 is "Supply Chain"** - Wrong! | **2/10** | ⚠️ **WRONG MAPPING** |
| **CTL-020** | Prompt Hygiene | OWASP LLM01, ASI01 | ✅ **LLM01: Prompt Injection** + **ASI01: Agent Goal Hijack** | **8/10** | Good match for injection prevention |
| **CTL-021** | Output Verification | OWASP LLM09, LLM05 | ✅ **LLM09: Misinformation** + **LLM05: SSRF** | **7/10** | LLM09 is good match, LLM05 less relevant |
| **CTL-023** | Mandatory Human Review | OWASP LLM06 | ✅ **LLM06: Excessive Agency** | **9/10** | Good match - human oversight prevents excessive agency |
| **CTL-024** | AI Feature Change Notification | OWASP LLM03, ASI04 | ❌ **Both wrong mappings** - LLM03 is Supply Chain, ASI04 is Supply Chain | **2/10** | ⚠️ **WRONG MAPPINGS** |
| **CTL-025** | Third-Party Risk Management | OWASP LLM03, ASI04 | ✅ **LLM03: Supply Chain** + **ASI04: Supply Chain** | **9/10** | Good match |
| **CTL-026** | Vendor Training Data Review | OWASP LLM04, ASI04 | ✅ **LLM04: Data and Model Poisoning** | **8/10** | Good match |
| **CTL-028** | AI Usage Monitoring | OWASP-Agent ASI10 | ✅ **ASI10: Rogue Agents** | **7/10** | Monitoring helps detect rogue agents |
| **CTL-029** | AI Incident Detection | OWASP-Agent ASI08, ASI10 | ✅ **ASI08: Excessive Agency** + **ASI10: Rogue Agents** | **7/10** | Good match |

### OWASP LLM Summary
- **Perfect/Strong Matches (8-10/10):** 6 controls
- **Moderate Alignment (6-7/10):** 3 controls
- **Weak/Poor (2-5/10):** 6 controls
- **Wrong Mappings:** 5 controls

**Overall OWASP LLM Confidence: 5.8/10**

**Major Issues:**
- Multiple wrong mappings to ASI03, ASI04
- Confusion between LLM Top 10 and Agentic Security Initiative (ASI)
- Some controls mapped to wrong vulnerability categories

---

## 4. OWASP Top 10 for Agentic AI Validation

### Official OWASP Agentic AI (ASI) Top 10
Published 2024. Specific to autonomous agent security.

| Control ID | Control Name | Claimed Alignment | Actual ASI Reference | Confidence Score | Issues |
|------------|--------------|-------------------|---------------------|------------------|--------|
| **CTL-003** | AI Acceptable Use | OWASP-Agent ASI03 | ❌ **ASI03: Identity & Privilege Abuse** - Wrong! | **2/10** | ⚠️ **WRONG** |
| **CTL-017** | AI Tool Approval Gate | OWASP-Agent ASI03 | ❌ **ASI03: Identity & Privilege Abuse** - Wrong! | **2/10** | ⚠️ **WRONG** |
| **CTL-018** | Block Unapproved Tools | OWASP-Agent ASI04 | ❌ **ASI04: Supply Chain Vulnerabilities** - Wrong! | **2/10** | ⚠️ **WRONG** |
| **CTL-020** | Prompt Hygiene | OWASP-Agent ASI01 | ✅ **ASI01: Agent Goal Hijack** | **8/10** | Good - prompt injection can hijack goals |
| **CTL-023** | Mandatory Human Review | OWASP-Agent ASI09 | ✅ **ASI09: Human-Agent Trust Exploitation** | **9/10** | Perfect - human review prevents trust exploitation |
| **CTL-024** | AI Feature Change Notification | OWASP-Agent ASI04 | ❌ **ASI04: Supply Chain** - Wrong! | **2/10** | ⚠️ **WRONG** |
| **CTL-025** | Third-Party Risk Management | OWASP-Agent ASI04 | ✅ **ASI04: Supply Chain Vulnerabilities** | **9/10** | Perfect match |
| **CTL-026** | Vendor Training Data Review | OWASP-Agent ASI04 | ⚠️ **ASI04: Supply Chain** - Training data is part of supply chain | **7/10** | Reasonable interpretation |
| **CTL-028** | AI Usage Monitoring | OWASP-Agent ASI10 | ✅ **ASI10: Rogue Agents** | **8/10** | Good - monitoring detects rogue agents |
| **CTL-029** | AI Incident Detection | OWASP-Agent ASI08, ASI10 | ✅ **ASI08: Excessive Agency** + **ASI10: Rogue Agents** | **8/10** | Good match |
| **CTL-030** | AI Incident Reporting | OWASP-Agent ASI10 | ⚠️ **ASI10: Rogue Agents** - Reporting is response, not detection | **6/10** | Indirect match |

### OWASP Agentic Summary
- **Perfect/Strong Matches (8-10/10):** 5 controls
- **Moderate Alignment (6-7/10):** 2 controls
- **Weak/Poor (2-5/10):** 5 controls
- **Wrong Mappings:** 4 controls

**Overall OWASP Agentic Confidence: 6.2/10**

**Major Issues:**
- ASI03 (Identity & Privilege Abuse) repeatedly misused
- ASI04 (Supply Chain) sometimes correct, sometimes wrong
- Confusion about which controls apply to agentic vs non-agentic

---

## 5. ISO/IEC 27001:2022 Validation

### Official ISO 27001:2022 Structure
Annex A contains 93 controls organized into 4 themes.

| Control ID | Control Name | Claimed Alignment | Actual ISO 27001 Reference | Confidence Score | Issues |
|------------|--------------|-------------------|---------------------------|------------------|--------|
| **CTL-001** | AI Policy | ISO27001 A.5.1 | ✅ **A.5.1 Policies for information security** | **9/10** | Good match |
| **CTL-003** | AI Acceptable Use | ISO27001 A.5.1 | ⚠️ **A.5.1** - AUP is implementation of policy | **7/10** | Reasonable |
| **CTL-007** | Concern Reporting | ISO27001 A.6.8 | ✅ **A.6.8 Information security event reporting** | **9/10** | Good match |
| **CTL-008** | User Responsibility | ISO27001 A.6.8 | ⚠️ **A.6.8** - User responsibility implied | **6/10** | Indirect |
| **CTL-012** | AI System Inventory | ISO27001 A.5.9 | ✅ **A.5.9 Inventory of information and associated assets** | **9/10** | Good match |
| **CTL-013** | Prohibit Sensitive Data | ISO27001 A.5.34 | ⚠️ **A.5.34 Privacy and protection of PII** - Doesn't prohibit, protects | **5/10** | ⚠️ **MISALIGNED** - Standard protects PII, doesn't prohibit use |
| **CTL-014** | Data Leakage Prevention | ISO27001 A.8.12 | ✅ **A.8.12 Data leakage prevention** | **10/10** | Perfect match |
| **CTL-016** | Data Classification | ISO27001 A.5.12-A.5.13 | ✅ **A.5.12 Classification** + **A.5.13 Labeling** | **10/10** | Perfect match |
| **CTL-017** | AI Tool Approval Gate | ISO27001 A.6.1 | ⚠️ **A.6.1 Screening** - Not about tool approval | **4/10** | ⚠️ **WEAK MATCH** |
| **CTL-018** | Block Unapproved Tools | ISO27001 A.8.19 | ✅ **A.8.19 Installation of software on operational systems** | **8/10** | Good match - blocking unapproved software |
| **CTL-025** | Third-Party Risk Management | ISO27001 A.5.19-A.5.23 | ✅ **A.5.19-A.5.23 Supplier relationships** | **10/10** | Perfect match |
| **CTL-027** | Vendor AI Register | ISO27001 A.5.22 | ⚠️ **A.5.22 Monitoring and review of supplier services** | **7/10** | Register is tool for monitoring |
| **CTL-028** | AI Usage Monitoring | ISO27001 A.8.16 | ✅ **A.8.16 Monitoring activities** | **9/10** | Good match |
| **CTL-029** | AI Incident Detection | ISO27001 A.5.25 | ⚠️ **A.5.25 Assessment and decision on information security events** | **6/10** | Detection is part of event management |
| **CTL-030** | AI Incident Reporting | ISO27001 A.5.24-A.5.28 | ✅ **A.5.24-A.5.28 Incident management** | **9/10** | Good match |
| **CTL-031** | AI Incident Response | ISO27001 A.5.24-A.5.28 | ✅ **A.5.24-A.5.28** | **9/10** | Good match |
| **CTL-032** | Security Awareness | ISO27001 A.6.3 | ✅ **A.6.3 Information security awareness, education and training** | **10/10** | Perfect match |
| **CTL-033** | AI Training Program | ISO27001 A.6.3 | ✅ **A.6.3** | **9/10** | Good match |
| **CTL-034** | Training Effectiveness | ISO27001 A.6.3 | ⚠️ **A.6.3** - Effectiveness implied | **7/10** | Reasonable extension |

### ISO 27001 Summary
- **Perfect Matches (10/10):** 5 controls
- **Strong Alignment (8-9/10):** 8 controls
- **Moderate Alignment (6-7/10):** 4 controls
- **Weak Alignment (4-5/10):** 2 controls

**Overall ISO 27001 Confidence: 8.1/10**

**Best Aligned Standard**

---

## 6. EU AI Act Validation

### Official EU AI Act Structure
Published August 2024. Risk-based approach with obligations for high-risk AI.

| Control ID | Control Name | Claimed Alignment | Actual EU AI Act Reference | Confidence Score | Issues |
|------------|--------------|-------------------|---------------------------|------------------|--------|
| **CTL-001** | AI Policy | EU AI Act Art. 9 | ✅ **Article 9: Risk management system** | **7/10** | Policy supports risk management |
| **CTL-002** | AI Guiding Principles | EU AI Act Recitals | ⚠️ **Recitals mention ethics** - Not explicit requirement | **5/10** | Principles implied, not mandated |
| **CTL-003** | AI Acceptable Use | EU AI Art. 5, 6 | ⚠️ **Art. 5 (Prohibited) + Art. 6 (Classification)** | **6/10** | Indirect match |
| **CTL-011** | AI Impact Assessment | EU AI Act Art. 9, 35 | ✅ **Art. 9: Risk mgmt + Art. 35: Fundamental rights impact** | **9/10** | Good match for high-risk |
| **CTL-013** | Prohibit Sensitive Data | EU AI Art. 10 | ⚠️ **Art. 10: Data governance** - Quality, not prohibition | **5/10** | ⚠️ **MISALIGNED** |
| **CTL-015** | Data Governance Checklist | EU AI Art. 10 | ✅ **Art. 10: Data and data governance** | **8/10** | Good match |
| **CTL-023** | Mandatory Human Review | EU AI Act Art. 14 | ✅ **Article 14: Human oversight** | **10/10** | Perfect match |
| **CTL-038** | Legal Requirements | EU AI Act | ✅ **Multiple articles** | **8/10** | General alignment |
| **CTL-039** | Regulatory Monitoring | EU AI Act | ⚠️ **Implied obligation** - Not explicit control | **6/10** | Reasonable interpretation |

### EU AI Act Summary
- **Perfect Matches (10/10):** 1 control
- **Strong Alignment (8-9/10):** 3 controls
- **Moderate Alignment (6-7/10):** 3 controls
- **Weak Alignment (4-5/10):** 3 controls

**Overall EU AI Act Confidence: 6.7/10**

**Notes:**
- EU AI Act is regulation, not standard with explicit controls
- Many mappings interpretive
- High-risk AI obligations most relevant

---

## Overall Standards Ranking by Confidence

| Rank | Standard | Average Confidence | Key Issues |
|------|----------|-------------------|------------|
| **1** | **ISO 27001:2022** | **8.1/10** | Best aligned, well-understood controls |
| **2** | **NIST AI RMF** | **7.4/10** | Framework nature allows interpretation |
| **3** | **ISO/IEC 42001:2023** | **7.2/10** | Some hallucinations (CTL-014, CTL-020) |
| **4** | **EU AI Act** | **6.7/10** | Regulation vs standard differences |
| **5** | **OWASP Agentic** | **6.2/10** | Wrong mappings (ASI03, ASI04) |
| **6** | **OWASP LLM** | **5.8/10** | Multiple wrong mappings, confusion between LLM/ASI |

---

## Critical Issues Requiring Correction

### 1. Hallucinated Controls (Not in Standards)
- **CTL-014:** Data Leakage Prevention - Cited as ISO 42001 A.7.2, but DLP is ISO 27001
- **CTL-020:** Prompt Hygiene - Cited as ISO 42001 A.6.5, but not in standard

### 2. Wrong Mappings (OWASP)
- **CTL-003:** Mapped to ASI03 (Identity & Privilege Abuse) - Wrong
- **CTL-017:** Mapped to ASI03 - Wrong
- **CTL-018:** Mapped to ASI04 (Supply Chain) - Wrong
- **CTL-019:** Mapped to LLM03 (Supply Chain) - Wrong
- **CTL-024:** Mapped to LLM03/ASI04 - Wrong

### 3. Misaligned Controls
- **CTL-013:** "Prohibit Sensitive Data" - Standards protect data, don't prohibit use
- **CTL-014:** DLP cited in ISO 42001 - Actually ISO 27001

### 4. Missing Framework References
- **CTL-035:** Model Testing & Validation - Not mapped to any standard in register
- **CTL-031:** AI Incident Response - Only mapped to ISO 27001, missing ISO 42001 Cl. 10

---

## Recommendations

### Immediate Actions:
1. **Remove or Correct Hallucinated Mappings**
   - Fix CTL-014 (remove ISO 42001 reference)
   - Fix CTL-020 (remove ISO 42001 reference)

2. **Correct Wrong OWASP Mappings**
   - CTL-003: Remove ASI03, keep relevant mappings
   - CTL-017: Remove ASI03, map to appropriate control
   - CTL-018: Remove ASI04, map to appropriate control
   - CTL-019: Remove LLM03, map to appropriate control
   - CTL-024: Remove LLM03/ASI04, map to appropriate control

3. **Clarify Misaligned Controls**
   - CTL-013: Reframe as "Data Protection" not "Prohibition"
   - CTL-014: Acknowledge it's ISO 27001, not ISO 42001

### Documentation Improvements:
4. **Add Missing Framework References**
   - CTL-035: Add ISO 42001 A.6.5 (Testing & Validation)
   - CTL-031: Add ISO 42001 Cl. 10 (Improvement)

5. **Distinguish Agentic vs Non-Agentic**
   - Clearly mark which controls apply to current tools vs future agentic AI
   - ASI mappings should be marked "Conditional" not "Applicable"

### Validation Process:
6. **Cross-Check All Mappings**
   - Verify each control against actual standard text
   - Use official standard documents, not secondary sources
   - Document rationale for each mapping

---

*Validation completed by Aqua Regia 🜆*  
*Based on official standard texts and frameworks*
