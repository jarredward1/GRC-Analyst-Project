# Corporate Cybersecurity Assessment Utilizing NIST Cybersecurity Framework (CSF) 2.0

> A comprehensive cybersecurity assessment for a fictional organization (Cypronetics), conducted using NIST CSF 2.0. Includes a pass/fail evaluation across all six core functions, current and target profile analysis, and a full remediation roadmap.

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Objectives](#-objectives)
- [Frameworks Applied](#️-frameworks-applied)
- [CSF Core Functions](#-csf-core-functions)
- [Maturity Tier Assessment](#-maturity-tier-assessment)
- [Current Status Report](#-current-status-report)
- [Assessment Findings and Recommendations](#-assessment-findings-and-recommendations)
  - [GOVERN](#govern)
  - [IDENTIFY](#identify)
  - [PROTECT](#protect)
  - [DETECT](#detect)
  - [RESPOND](#respond)
  - [RECOVER](#recover)
- [Conclusion](#-conclusion)
- [Author](#-author)

---

## 📌 Overview

For this project I was tasked with analyzing a fictional organization's (Cypronetics) cybersecurity posture and designing a comprehensive security program utilizing [NIST CSF 2.0](https://www.nist.gov/publications/nist-cybersecurity-framework-csf-20). Using a current status report compiled from employee and stakeholder interviews, I conducted a pass/fail assessment across all CSF core functions and delivered recommendations for improvement, including a stakeholder presentation and a full remediation plan.

---

## 🎯 Objectives

- Evaluate Cypronetics's current cybersecurity posture against NIST CSF 2.0
- Identify deficiencies across all six core functions
- Determine current and target maturity tier profiles
- Deliver actionable recommendations for each subcategory
- Present findings and a remediation roadmap to stakeholders

---

## 🛠️ Frameworks Applied

| Framework | Purpose |
|-----------|---------|
| **NIST CSF 2.0** | Primary assessment and remediation framework |
| **NIST SP 800-53** | Control verification and policy implementation |
| **MITRE ATT&CK** | SIEM alignment and threat detection guidance |
| **OWASP** | Secure design principles for risk management |

---

## 📊 CSF Core Functions

The CSF Core Functions (GOVERN, IDENTIFY, PROTECT, DETECT, RESPOND, and RECOVER) organize cybersecurity outcomes at their highest level.

| Core Function | Description |
|---------------|-------------|
| ![GOVERN](https://github.com/user-attachments/assets/c536c78f-b8d2-4988-a1ad-ea1b0222bd41) | The organization's cybersecurity risk management strategy, expectations, and policy are established, communicated, and monitored. |
| ![IDENTIFY](https://github.com/user-attachments/assets/bd218bc5-9048-4d91-96fd-77aba367d87b) | The organization's current cybersecurity risks are understood. |
| ![PROTECT](https://github.com/user-attachments/assets/f6554061-0d01-49e9-91df-b102eb4b8ac7) | Safeguards to manage the organization's cybersecurity risks are used. |
| ![DETECT](https://github.com/user-attachments/assets/26e591c9-9ee6-454f-9f5b-37062bec1d0c) | Possible cybersecurity attacks and compromises are found and analyzed. |
| ![RESPOND](https://github.com/user-attachments/assets/bfdf2e21-ced1-4767-8ac6-4ec982b6f5e3) | Actions regarding a detected cybersecurity incident are taken. |
| ![RECOVER](https://github.com/user-attachments/assets/10ef5d64-da8b-41df-a0fe-56acb244fd1c) | Assets and operations affected by a cybersecurity incident are restored. |

---

## 📈 Maturity Tier Assessment

![Tiers](https://github.com/user-attachments/assets/a9b93ba7-a2a2-4cdc-954f-8016f3df6e58)

The rigor of an organization's cybersecurity risk governance and management practices can be categorized according to a table of tiers as outlined in CSF 2.0 Profiles and Tiers.

![image](https://github.com/user-attachments/assets/60704a33-4b7f-4925-8eef-4084d5fa484c)

**Cypronetics's current profile is identified as Tier 1: Partial.**

| Tier | Cybersecurity Risk Governance | Cybersecurity Risk Management |
|------|-------------------------------|-------------------------------|
| Tier 1: Partial | Application of the organizational cybersecurity risk strategy is managed in an ad hoc manner. Prioritization is ad hoc and not formally based on objectives or threat environment. | There is limited awareness of cybersecurity risks at the organizational level. The organization implements cybersecurity risk management on an irregular, case-by-case basis. |

**Target profile for Cypronetics: Tier 4: Adaptive.**

| Tier | Cybersecurity Risk Governance | Cybersecurity Risk Management |
|------|-------------------------------|-------------------------------|
| Tier 4: Adaptive | There is an organization-wide approach to managing cybersecurity risks that uses risk-informed policies, processes, and procedures to address potential cybersecurity events. Executives monitor cybersecurity risks in the same context as financial and other organizational risks. | The organization adapts its cybersecurity practices based on previous and current cybersecurity activities, including lessons learned and predictive indicators. Cybersecurity information is constantly shared throughout the organization and with authorized third parties. |

At all times the question should be asked whether data is kept *Confidential*, its *Integrity* is upheld, and is readily *Available* and what risks and vulnerabilities present a danger to this '[CIA Triad](https://www.nccoe.nist.gov/publication/1800-26/VolA/index.html)'.

![image](https://github.com/user-attachments/assets/5b8e35de-2c04-4de8-a82c-bb526a3f6f5c)

---

## 🏢 Current Status Report

<details close>
<summary><h3>Cypronetics current status report (click here)</h3></summary>

**Current Cypronetics cybersecurity team:**
- Cyber security analyst: generalist, responds to cyber incidents as they come. Reports to Cypronetics's IT manager.
- Network engineer: manages the firewalls. Reports to the Network Team Leader.
- Cyber Security Consultant: your new role at Cypronetics. You will initially report to the IT manager.

**Cypronetics current cyber security controls:**
- Organisational governance:
  - CEO has a clear business strategy for the business. However, roles and responsibilities for cybersecurity have not been defined. There is no cybersecurity strategy.
- Asset Management:
  - The IT team has a spreadsheet with serial numbers of laptops including model and warranty details.
  - Cypronetics uses Microsoft Office 365 and relies exclusively on SaaS applications. All data is in Microsoft Azure cloud.
  - The IT team uses a Secure Operating Environment (SOE) to image all laptops with the latest Windows version.
- Business Continuity and Disaster Recovery:
  - The IT team conducts regular disaster recovery testing with clear, documented business continuity plans and periodic backup testing.
- Vulnerability Management:
  - Cypronetics has purchased Qualys vulnerability scanner but uses it on an ad-hoc basis. No formal vulnerability management program is in place. A large number of high and severe vulnerabilities have been reported.
- Risk Management:
  - Cypronetics has a risk team that performs financial risk activities. There is no technology or cyber risk process.
- Third Party Risk Management:
  - No third-party risk management is performed. Contracts are reviewed by procurement and finance, not IT.
- Identity and Access Management:
  - Microsoft Active Directory is used to manage users and groups. No privileged access management solution is in place. Admin account password is shared with senior IT members. No two-factor authentication. Complex login passwords are used. Employees use VPN for remote access.
- Network Security:
  - Palo Alto Next Gen firewalls are in place, configured and audited annually by the network team. Up-to-date network diagrams including cloud environment. Network is segmented using VLANs.
- Physical Security:
  - Highly secure facility with CCTV, 24/7 monitoring, and extensive employee vetting.
- Data Security:
  - No DLP solution. All data resides in Microsoft Azure and Office 365. Key critical application is a SaaS service from Horizon Labs.
- Policy:
  - One generic IT policy in place. No formal information security policy or data governance policies.
- Cyber Security Detection and Response:
  - No detection or response capability. IT team responds to Microsoft Defender alerts only. No SIEM in place.
- Security Education and Awareness:
  - All employees complete an induction web training module with basic cybersecurity instructions.

</details>

---

## 🔍 Assessment Findings and Recommendations

Utilizing CSF core functions as a guide, an assessment of Cypronetics identified many deficiencies. Recommendations are provided after each subcategory.

---

### GOVERN

![GOVERN](https://github.com/user-attachments/assets/a9b93ba7-a2a2-4cdc-954f-8016f3df6e58)

<details close>
<summary><h3>NIST Cybersecurity Framework 2.0 pass/fail logs (click here)</h3></summary>

![Pass/Fail 1](https://github.com/user-attachments/assets/586dd539-f042-4bea-b9d2-290b8e445571)
![Pass/Fail 2](https://github.com/user-attachments/assets/c0c4e42a-7736-48b1-ac59-92604fef17ca)

</details>

---

### IDENTIFY

![IDENTIFY](https://github.com/user-attachments/assets/9dc5bda1-08f0-4d90-b806-34621a19553a)

<details close>
<summary><h3>NIST Cybersecurity Framework 2.0 pass/fail logs (click here)</h3></summary>

![Pass/Fail 1](https://github.com/user-attachments/assets/586dd539-f042-4bea-b9d2-290b8e445571)
![Pass/Fail 2](https://github.com/user-attachments/assets/c0c4e42a-7736-48b1-ac59-92604fef17ca)

</details>

#### Asset Management
- *Physical devices and systems ARE properly inventoried, however no IP address identified.* No access agents identified, limiting vulnerability scanner scope.
- *External information systems are NOT properly catalogued.* No third-party risk management or IT involvement.
- *Resources are NOT prioritized based on classification, criticality, and business value.* No asset classification process exists.
- *Cybersecurity roles and responsibilities for the workforce and third-party stakeholders are NOT established.*

A vulnerability management policy needs to be implemented with access agents installed on all network-connected devices. Third-party risk management policy needs to be implemented. Assets need to be labeled using a sensitivity or criticality classification determined by the Maximum Tolerable Outage matrix.

![image](https://github.com/user-attachments/assets/0fd3f160-1f11-4da1-a781-d0837b1115c7)

`(RPO=recovery point objective, RTO=recovery time objective, WRT=working recovery time)`

#### Business Environment
- *The organization's role in the supply chain is NOT identified and communicated.*

Clear documentation is needed outlining their role within the supply chain, including mapping and classifying third-party suppliers based on criticality and sensitivity.

#### Governance
- *Organizational information security policy is NOT established.*
- *Information security roles and responsibilities are NOT coordinated with internal roles and external partners.*
- *Legal and regulatory requirements regarding cybersecurity are NOT understood and managed.*
- *Governance and risk management processes DO NOT address cybersecurity risk.*

A formal cyber and information security policy needs to be established. Roles, responsibilities, and regulatory requirements need to be documented and communicated with internal and external stakeholders. A comprehensive risk management process needs to be established with direct board member oversight.

#### Risk Assessment and Risk Management Strategy
- *Asset vulnerabilities are NOT identified and documented.* Scans are conducted ad-hoc with no established procedures.
- *Threat and vulnerability information is NOT received from information sharing forums.*
- *Threats, both internal and external, are NOT identified and documented.*
- *Potential business impacts and likelihoods are NOT identified.*
- *Risk responses are NOT identified and prioritized.*
- *Organizational risk tolerance is undetermined and NOT clearly expressed.*

A full-scale cyber security risk management policy needs to be implemented utilizing **[OWASP](https://owasp.org/)** secure design principles and [NIST SP 800-53](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final) for control verification. A risk matrix should be used to establish risk tolerance and priority.

![Screenshot 2024-09-06 155149](https://github.com/user-attachments/assets/88309da8-792e-4e3d-a6ed-d7c293cfc655)

---

### PROTECT

![PROTECT](https://github.com/user-attachments/assets/eaa0f70b-acb1-43ba-9186-53f4c406875c)

<details close>
<summary><h3>NIST Cybersecurity Framework 2.0 pass/fail logs (click here)</h3></summary>

![Pass/Fail 1](https://github.com/user-attachments/assets/83ff0872-74e1-4969-a1f2-29a639abb176)
![Pass/Fail 2](https://github.com/user-attachments/assets/f36bc530-31e3-4425-a67d-2a70586aa605)
![Pass/Fail 3](https://github.com/user-attachments/assets/cac40a40-e19a-464c-a819-e8f1651e5231)

</details>

#### Access Controls
- *Identities and credentials are NOT adequately managed.* No MFA. No offboarding procedures. No periodic access reviews.
- *Physical access to assets is NOT managed and protected.* No verified entry/exit logs, biometrics, or access management policy.
- *Remote access is NOT adequately managed.* No two-factor authentication for VPN.
- *Access permissions are NOT managed incorporating least privilege and separation of duties.*

An Identity and Access Management (IAM) policy needs to be established covering MFA, access control lists, role-based access control, on- and off-boarding procedures, and remote access directives including 2FA.

#### Awareness Training
- *All users are NOT informed and trained.* No regular training. Insufficient onboarding training. No third-party training protocol.
- *Privileged users DO NOT understand roles and responsibilities.* No privileged access management in place.
- *Senior executives DO NOT understand roles and responsibilities.*

A training and education program needs to be established, run periodically, and kept up to date. Training should extend to third-party providers through TPRM. Dedicated training for executives and board members needs to be established.

#### Data Security
- *Data-at-rest is NOT adequately protected.* No data classification or DLP strategy implemented.
- *Data-in-transit is NOT adequately protected.* No USB data transfer limitations established.
- *Assets are NOT formally managed throughout removal, transfers, and disposition.*

A Data Loss Prevention method needs to be configured. Data needs to be classified and labeled. Movement and exfiltration of data need to be monitored. Asset and data disposal policies need to be implemented.

#### Information Protection Processes and Procedures
- *No configuration change control processes are in place.*
- *Data is NOT destroyed according to policy.* No data disposal policy in place.
- *No vulnerability management plan is developed or implemented.*

Configuration change protocols, physical security policies, data disposal policies, and personnel offboarding procedures all need to be implemented and documented. A formal vulnerability management program needs to be established.

#### Protective Technology
- *Audit/log records are NOT determined, documented, implemented, or reviewed according to policy.* No SIEM in place.
- *Removable media is NOT protected and its use restricted according to policy.*
- *Communications and control networks are NOT adequately protected.*

A Security Information and Event Management (SIEM) needs to be implemented and aligned with [MITRE ATT&CK](https://attack.mitre.org/). Policy needs to be established and personnel appointed for monitoring.

---

### DETECT

![DETECT](https://github.com/user-attachments/assets/2a5d2bd2-ba9b-4cff-84c2-840f73c4633b)

<details close>
<summary><h3>NIST Cybersecurity Framework 2.0 pass/fail logs (click here)</h3></summary>

![Pass/Fail 1](https://github.com/user-attachments/assets/e8f4d360-6015-451c-8484-3fc6b868b63b)
![Pass/Fail 2](https://github.com/user-attachments/assets/7fc2cbd1-0dcd-4818-8413-c17ef30d0716)

</details>

#### Anomalies and Events
Implement a SIEM to capture and monitor network traffic. Monitor logs and events, analyze threats, classify low/medium/high impact events based on criticality, and establish escalation points.

#### Security Continuous Monitoring
Implement a SIEM to capture and monitor network traffic. Merely monitoring traffic and alerts through Microsoft Defender is critically inadequate. Implement detection and response procedures, a formal third-party risk management policy, and a formal vulnerability management policy.

#### Detection Processes
Detection and response capabilities need to be established with clearly defined roles and responsibilities. Separation of duties between the IT department and cybersecurity department should be considered. Periodic penetration testing should be used to verify the robustness of the security posture.

---

### RESPOND

![RESPOND](https://github.com/user-attachments/assets/0e5fa430-0cea-4d22-be43-912381a82917)

<details close>
<summary><h3>NIST Cybersecurity Framework 2.0 pass/fail logs (click here)</h3></summary>

![Pass/Fail 1](https://github.com/user-attachments/assets/ef22e6a8-8635-47a4-abfc-80181246c01c)

</details>

#### Response Planning
A cybersecurity response process and policy needs to be established.

#### Communications
Incident response activities need to be determined and communicated with internal and external stakeholders. Include all contact details, establish thresholds and escalation points, and share findings with industry peers.

#### Analysis
Ensure analysis is conducted to determine adequate response and support recovery activities. Document criticality of incidents. Consider the ability for forensic investigations when needed.

#### Mitigation
- Ensure incident response plans follow a standard that ensures incidents are contained and mitigated (SANS incident response plans).
- Establish a vulnerability management program to aid in identifying and categorizing new, known, and unknown vulnerabilities.
- Establish a process for dealing with zero-day vulnerabilities.

#### Improvements
Analyze, test, and update incident response plans continuously.

---

### RECOVER

![RECOVER](https://github.com/user-attachments/assets/b595cac7-1881-4388-b3ac-4e5f59a099fc)

<details close>
<summary><h3>NIST Cybersecurity Framework 2.0 pass/fail logs (click here)</h3></summary>

![Pass/Fail 1](https://github.com/user-attachments/assets/92ba5adc-b78e-447e-bba8-c2d2103bdefc)

</details>

#### Communications
Coordinate restoration activities with internal and external parties such as coordinating centers, ISPs, owners of attacking systems, victims, other CSIRTs, and vendors. Consider the need for a reputational damage mitigation policy.

---

## ✅ Conclusion

After investigating Cypronetics's security posture, findings were analyzed and overlaid with NIST CSF 2.0. Relevant security frameworks including MITRE ATT&CK, NIST SP 800-53, and OWASP were utilized to compile a comprehensive roadmap toward a secure security infrastructure.

---

## 👤 Author

**Jarred Ward**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?logo=linkedin&style=for-the-badge)](https://www.linkedin.com/in/jarredward1/)
