# Incident Response Playbook  
**Author:** Kelly Esteves  
**Role:** Cybersecurity Analyst
**Created:** July 2025

---

## 1. Purpose  
This playbook provides structured, actionable guidance for managing cybersecurity incidents in an enterprise IT environment. It is designed to improve readiness, reduce risk, and comply with global frameworks such as NIST and emerging regulatory standards.

---

## 2. 2025 Cyber Threat Landscape

- **Ransomware as Operational Disruption**: 92% of ransomware incidents in 2024 involved data exfiltration and deliberate operational disruption. ([Palo Alto Networks Report](https://www.paloaltonetworks.com/perspectives/the-rising-stakes-of-cyber-resilience-what-the-2025-global-incident-response-report-means-for-business-leaders))
- **Retail & Smishing Attacks**: Threat actors like Scattered Spider use phishing, smishing, and remote tools like AnyDesk to breach retail systems. ([TechRadar](https://www.techradar.com/pro/i-am-a-cybersecurity-pro-and-heres-the-most-powerful-strategy-criminals-are-using-against-retailers-right-now))
- **Zero-Day Exploits in Infrastructure**: Attacks on Microsoft SharePoint servers by China-linked actors impacted over 100 organizations. ([Politico](https://www.politico.com/news/2025/07/22/microsoft-sharepoint-hack-china-federal-agencies-00467254))
- **Readiness & Response Simulations**: Regular red/blue team exercises are now key to organizational resilience. ([TechRadar](https://www.techradar.com/pro/you-have-to-find-the-needle-in-the-haystack-how-preparation-can-save-your-business-in-a-cyberattack))
- **Regulatory Changes**: New York now mandates cyber incident reporting within 72 hours. ([WSJ](https://www.wsj.com/articles/new-york-orders-local-governments-to-start-reporting-cyberattacks-c5f20b09))

---

## 3. Framework: NIST SP 800-61r2 & CSF 2.0

### Phases:
1. **Preparation**
2. **Detection and Analysis**
3. **Containment, Eradication, and Recovery**
4. **Post-Incident Activity**

References:  
- [NIST Incident Handling Guide (SP 800-61r2)](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r2.pdf)  
- [Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework)

---

## 4. Common Incident Playbooks

### 4.1 Ransomware  
- **Detect**: File encryption, outbound traffic anomalies  
- **Contain**: Disconnect host, isolate segments  
- **Eradicate**: Full antivirus/EDR sweep  
- **Recover**: Clean restore, credential rotation  
- **Review**: Update policy, patch gaps

### 4.2 Phishing  
- **Detect**: User reports, DLP alerts  
- **Contain**: Delete emails, block sender  
- **Eradicate**: Revoke access tokens  
- **Recover**: Password resets, MFA enforcement  
- **Review**: User awareness session

### 4.3 Unauthorized Access  
- **Detect**: Unusual logins/IPs  
- **Contain**: Disable accounts, block IP  
- **Eradicate**: Patch, update configs  
- **Recover**: Reinstate from backup  
- **Review**: Audit access control

---

## 5. Roles & Responsibilities

| Role           | Responsibilities                                                                 |
|----------------|----------------------------------------------------------------------------------|
| IT Support     | First response, isolation, ticket creation                                       |
| Security Team  | Forensics, malware analysis, remediation planning                                |
| Management     | Communication, decision making, legal and regulatory follow-up                   |

---

## 6. Communication Plan

- Document incidents in ticketing systems (e.g., Jira)
- Escalate based on severity (minor → internal / critical → CISO, Legal)
- Notify users as needed using standard templates
- Submit legal disclosures if breach thresholds are met

---

## 7. Documentation Requirements

Each incident must include:
- Time, type, and scope
- Detection method
- Affected systems
- Actions taken and by whom
- Root cause and postmortem summary

---

## 8. Tools & Technology Stack

| Category               | Tool/Platform                                               |
|------------------------|-------------------------------------------------------------|
| EDR & Antivirus        | [CrowdStrike], [Defender] |
| Ticketing              | [Jira]             |
| Monitoring             | [Grafana], [Zabbix] |
| SIEM / SOAR            | [Wazuh], [Splunk], [Elastic] |
| Threat Intelligence    | [CISA Alerts], [M-Trends] |

---

## 9. Review Cycle

- Conduct simulation exercises twice per year  
- Update documentation after each real incident  
- Perform tabletop scenarios for critical systems quarterly  
- Audit the entire IR plan every 6 months

---

## 10. References

- [Palo Alto 2025 IR Report](https://www.paloaltonetworks.com/perspectives/the-rising-stakes-of-cyber-resilience-what-the-2025-global-incident-response-report-means-for-business-leaders)  
- [TechRadar: Needle in Haystack](https://www.techradar.com/pro/you-have-to-find-the-needle-in-the-haystack-how-preparation-can-save-your-business-in-a-cyberattack)  
- [Politico: SharePoint Hack](https://www.politico.com/news/2025/07/22/microsoft-sharepoint-hack-china-federal-agencies-00467254)  
- [CISA SIEM Guidance](https://www.cisa.gov/news-events/alerts/2025/05/27/new-guidance-siem-and-soar-implementation)  
- [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework)  
- [WSJ NY Reporting Law](https://www.wsj.com/articles/new-york-orders-local-governments-to-start-reporting-cyberattacks-c5f20b09)
