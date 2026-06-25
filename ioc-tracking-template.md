# IOC Tracking Template

**Version:** 1.0  
**Last Updated:** June 2026  
**Owner:** Information Security Team  
**Classification:** Confidential  

---

## What is an IOC?

An Indicator of Compromise (IOC) is a piece of forensic evidence that suggests a system or network has been breached or targeted. IOCs are used to detect, contain, and prevent cyber attacks.

---

## IOC Categories

| Category | Examples |
|---|---|
| IP Addresses | Malicious IPs used for C2 communication or scanning |
| Domain Names | Phishing domains, malware distribution sites |
| URLs | Specific malicious URLs used in attacks |
| File Hashes | MD5, SHA1, SHA256 hashes of malicious files |
| Email Addresses | Sender addresses used in phishing campaigns |
| Email Subject Lines | Subject lines associated with phishing campaigns |
| File Names | Names of malicious files or tools |
| Registry Keys | Malicious registry entries for persistence |
| User Agents | Malicious browser or tool user agent strings |
| CVE Numbers | Known vulnerabilities being actively exploited |

---

## IOC Register

Use this table to log and track all indicators of compromise:

| IOC ID | Date Added | IOC Type | IOC Value | Threat Actor | Campaign | Confidence | Source | Action Taken | Status | Date Resolved |
|---|---|---|---|---|---|---|---|---|---|---|
| IOC-001 | | IP Address | | | | High / Med / Low | | Blocked / Monitored | Active / Resolved | |
| IOC-002 | | Domain | | | | High / Med / Low | | Blocked / Monitored | Active / Resolved | |
| IOC-003 | | File Hash | | | | High / Med / Low | | Blocked / Monitored | Active / Resolved | |
| IOC-004 | | Email Address | | | | High / Med / Low | | Blocked / Monitored | Active / Resolved | |
| IOC-005 | | URL | | | | High / Med / Low | | Blocked / Monitored | Active / Resolved | |

---

## Confidence Ratings

| Rating | Description |
|---|---|
| High | Confirmed malicious from trusted source or internal investigation |
| Medium | Likely malicious based on behaviour or multiple sources |
| Low | Potentially malicious, requires further investigation |

---

## IOC Lifecycle

**Active** — IOC is current and blocking or monitoring rules are in place  
**Under Review** — IOC is being investigated  
**Expired** — IOC is no longer considered a current threat  
**Resolved** — IOC was associated with an incident that has been resolved  
**False Positive** — IOC was incorrectly identified as malicious  

---

## IOC Sources

| Source | Type | URL | Reliability |
|---|---|---|---|
| AlienVault OTX | Free feed | otx.alienvault.com | High |
| Abuse.ch | Free feed | abuse.ch | High |
| MalwareBazaar | File hashes | bazaar.abuse.ch | High |
| PhishTank | Phishing URLs | phishtank.org | High |
| Shodan | IP intelligence | shodan.io | High |
| VirusTotal | File and URL analysis | virustotal.com | High |
| MITRE ATT&CK | TTP framework | attack.mitre.org | High |
| CISA Advisories | Government advisories | cisa.gov | High |

---

## IOC Sharing Guidelines

- Share IOCs with industry peers and threat sharing groups where permitted
- Remove any sensitive business context before sharing externally
- Use STIX/TAXII format for structured IOC sharing where possible
- Do not share IOCs that could identify affected individuals or systems externally

---

## Monthly IOC Review Checklist

- [ ] Review all active IOCs for continued relevance
- [ ] Remove or expire IOCs older than 90 days unless still active
- [ ] Check for new IOCs from subscribed feeds
- [ ] Update blocking rules based on new IOCs
- [ ] Report IOC summary to security team
- [ ] Document any IOCs linked to active incidents

---

*Developed by TrustGrid Technology Limited — github.com/TechShieldOlamide*
