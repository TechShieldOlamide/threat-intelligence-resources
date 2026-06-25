# Threat Intelligence Framework

**Version:** 1.0  
**Last Updated:** June 2026  
**Owner:** Information Security Team  
**Review Date:** June 2027  
**Classification:** Internal  

---

## 1. Purpose

This framework provides a structured approach to building and operating a threat intelligence programme. It is designed for organisations that want to move from reactive security to proactive threat-informed defence.

---

## 2. Threat Intelligence Lifecycle

### Phase 1 — Planning and Direction

Define what you need to know and why.

- Identify key assets that need protecting
- Define intelligence requirements based on business risk
- Identify stakeholders who will consume the intelligence
- Set collection priorities

**Key questions:**
- What are our most critical assets?
- Who is likely to target us and why?
- What threats would have the highest business impact?

---

### Phase 2 — Collection

Gather raw data from relevant sources.

**Internal sources:**
- Security logs and SIEM alerts
- Endpoint detection alerts
- Firewall and network logs
- Incident response findings
- Vulnerability scan results

**External sources:**
- Open source threat intelligence feeds
- Industry threat sharing groups
- Government and regulatory advisories
- Dark web monitoring
- Vendor threat reports

---

### Phase 3 — Processing

Convert raw data into usable intelligence.

- Normalise data from different sources into a consistent format
- Remove duplicates and false positives
- Enrich IOCs with additional context
- Tag and categorise findings by threat type and severity
- Store processed intelligence in a centralised repository

---

### Phase 4 — Analysis

Turn processed data into actionable intelligence.

- Identify patterns and trends across collected data
- Map threat actor behaviour to MITRE ATT&CK framework
- Assess relevance and credibility of each intelligence item
- Determine likelihood and impact for your organisation
- Prioritise threats based on business risk

---

### Phase 5 — Dissemination

Share intelligence with the right people in the right format.

| Audience | Format | Frequency |
|---|---|---|
| Executive leadership | Strategic summary | Monthly |
| Security team | Technical IOCs and TTPs | Daily or as needed |
| IT team | Actionable remediation guidance | As needed |
| Wider staff | Awareness bulletins | Monthly |

---

### Phase 6 — Feedback

Continuously improve the programme.

- Collect feedback from intelligence consumers
- Assess whether intelligence led to action
- Identify gaps in collection or analysis
- Update intelligence requirements based on feedback
- Review and improve processes quarterly

---

## 3. Intelligence Types

| Type | Description | Example |
|---|---|---|
| Strategic | High level trends for executive decision making | Nation state threats to financial sector |
| Operational | Details about specific planned attacks | Phishing campaign targeting Nigerian fintechs |
| Tactical | TTPs of threat actors | Techniques used by a specific ransomware group |
| Technical | Specific IOCs for detection and blocking | Malicious IP addresses and file hashes |

---

## 4. Intelligence Requirements Template

Use this to define what intelligence your organisation needs:

| Priority | Intelligence Requirement | Business Justification | Collection Source | Review Date |
|---|---|---|---|---|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |

---

## 5. MITRE ATT&CK Alignment

Map identified threats to the MITRE ATT&CK framework to understand attacker behaviour:

| Tactic | Technique | Observed | Mitigation |
|---|---|---|---|
| Initial Access | Phishing | Yes / No | |
| Execution | Malicious Scripts | Yes / No | |
| Persistence | Registry Run Keys | Yes / No | |
| Privilege Escalation | Token Manipulation | Yes / No | |
| Defence Evasion | Obfuscated Files | Yes / No | |
| Credential Access | Brute Force | Yes / No | |
| Lateral Movement | Pass the Hash | Yes / No | |
| Exfiltration | Encrypted Channel | Yes / No | |

Full framework available at attack.mitre.org

---

## 6. Programme Maturity Model

| Level | Description |
|---|---|
| Level 1 — Initial | Ad hoc threat intelligence, no formal process |
| Level 2 — Developing | Some collection and analysis, limited sharing |
| Level 3 — Defined | Formal programme, regular reporting, IOC management |
| Level 4 — Managed | Integrated with security operations, proactive hunting |
| Level 5 — Optimising | Continuous improvement, sharing with industry peers |

---

*Developed by TrustGrid Technology Limited — github.com/TechShieldOlamide*
