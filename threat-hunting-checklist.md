# Threat Hunting Checklist

**Version:** 1.0  
**Last Updated:** June 2026  
**Owner:** Information Security Team  
**Classification:** Internal  

---

## What is Threat Hunting?

Threat hunting is the proactive process of searching through networks, endpoints, and datasets to detect threats that have evaded existing security controls. Unlike reactive security, threat hunting assumes a breach may already have occurred and looks for evidence of attacker activity.

---

## Before You Start

- [ ] Define the scope of this hunt
- [ ] Identify the hypothesis you are testing
- [ ] Confirm access to required log sources
- [ ] Document baseline normal behaviour for the environment
- [ ] Assign a hunt lead and document the team
- [ ] Set a time period for the hunt

**Hunt hypothesis:**
[What threat or attacker behaviour are you looking for?]

**Scope:**
[What systems, networks, or time periods are in scope?]

---

## 1. Network Traffic Analysis

- [ ] Review firewall logs for unusual outbound connections
- [ ] Identify connections to known malicious IP addresses or domains
- [ ] Look for large or unusual data transfers
- [ ] Check for connections on unusual ports
- [ ] Identify DNS queries to newly registered or suspicious domains
- [ ] Look for beaconing patterns suggesting C2 communication
- [ ] Review VPN logs for unusual access times or locations
- [ ] Check for lateral movement between internal systems

---

## 2. Endpoint Analysis

- [ ] Review process creation logs for unusual processes
- [ ] Check for processes running from unusual locations
- [ ] Identify scripts running from temp or download directories
- [ ] Look for unusual parent-child process relationships
- [ ] Check for persistence mechanisms in startup folders and registry
- [ ] Review scheduled tasks for unauthorised entries
- [ ] Check for unsigned or recently created executables
- [ ] Look for tools associated with living off the land attacks

---

## 3. User Account Analysis

- [ ] Review authentication logs for unusual login times
- [ ] Check for logins from unusual locations or IP addresses
- [ ] Identify accounts with multiple failed login attempts
- [ ] Look for privilege escalation attempts
- [ ] Check for new accounts created without authorisation
- [ ] Review admin account activity for unusual behaviour
- [ ] Identify dormant accounts that have recently become active
- [ ] Check for password changes outside normal patterns

---

## 4. Email and Phishing Analysis

- [ ] Review email gateway logs for suspicious inbound messages
- [ ] Check for emails with malicious attachments or links
- [ ] Identify bulk email activity from internal accounts
- [ ] Look for email forwarding rules set up without authorisation
- [ ] Check for emails sent to external addresses containing sensitive data
- [ ] Review emails from newly registered or lookalike domains

---

## 5. Cloud and SaaS Analysis

- [ ] Review cloud access logs for unusual activity
- [ ] Check for new admin accounts or permission changes
- [ ] Identify data downloads or exports outside normal patterns
- [ ] Look for API calls from unusual IP addresses
- [ ] Check for disabled security controls or logging
- [ ] Review storage bucket access for public exposure

---

## 6. Application and Database Analysis

- [ ] Review application logs for unusual queries or access patterns
- [ ] Check for SQL injection attempts in application logs
- [ ] Identify unusual API call volumes or patterns
- [ ] Look for access to sensitive data outside normal business hours
- [ ] Check for bulk data exports from databases
- [ ] Review failed authentication attempts on applications

---

## 7. Indicators of Compromise Check

- [ ] Run known IOCs against all available log sources
- [ ] Check file hashes against malware databases
- [ ] Scan for known malicious domains in DNS logs
- [ ] Check for known malicious IP addresses in network logs
- [ ] Review for CVEs being actively exploited in the wild

---

## Hunt Findings Log

| ID | Finding | System Affected | Severity | Evidence | Recommended Action | Status |
|---|---|---|---|---|---|---|
| 001 | | | | | | |
| 002 | | | | | | |
| 003 | | | | | | |

---

## Hunt Summary

**Hunt Start Date:**  
**Hunt End Date:**  
**Systems Reviewed:**  
**Log Sources Reviewed:**  
**Findings Identified:**  
**Critical Findings:**  
**Actions Taken:**  

---

## Post Hunt Actions

- [ ] Document all findings and evidence
- [ ] Escalate critical findings to incident response team
- [ ] Update IOC register with new indicators identified
- [ ] Tune detection rules based on hunt findings
- [ ] Share findings with security team
- [ ] Schedule follow up hunt if required
- [ ] Update threat hunting checklist based on lessons learned

---

*Developed by TrustGrid Technology Limited — github.com/TechShieldOlamide*
