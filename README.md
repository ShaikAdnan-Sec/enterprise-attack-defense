# Enterprise Attack & Defense Lab

## 1. Project Objective

To design, deploy, and secure a miniature enterprise environment. This project demonstrates end-to-end security engineering by deliberately attacking the infrastructure, building detections for those attacks, and automating the incident response lifecycle.

## 2. Architecture

(Diagram placeholder: Windows Domain Controller, Windows Client, Linux Server, Web App, Centralized Logging)

## 3. Threat Model

- **Assets:** Internal credentials, application databases, administrative access.
- **Adversaries:** External attacker compromising a web app, internal user privilege escalation.
- **Attack Paths:** Web Application -> Initial Access -> Credential Discovery -> Privilege Escalation -> Lateral Movement -> Domain Compromise.

## 4. Initial Technology Choices

- **Infrastructure:** Linux, Windows Server, Active Directory, Docker
- **Automation:** Python, PowerShell, Ansible, Terraform
- **Monitoring:** Centralised logging / SIEM
- **Version Control:** Git

## 5. Attack Scenarios

1. **Initial Access:** Exploiting a vulnerable web application to gain a foothold.
2. **Privilege Escalation:** Moving from a low-privileged account to administrative access.
3. **Lateral Movement:** Pivoting from the compromised web server to an internal domain machine.

## 6. Defensive Objectives

- Implement centralised logging across all endpoints.
- Develop detection engineering rules based on attack telemetry.
- Document triage and investigation workflows for generated alerts.
- Execute and document incident response and remediation steps.

## 7. Definition of Done

- [ ] Environment reproducibly deploys via Infrastructure as Code.
- [ ] Threat model documented.
- [ ] Three attack scenarios implemented and validated.
- [ ] Telemetry successfully collected in a centralised logging platform.
- [ ] Detection rules implemented for each attack scenario.
- [ ] Investigations documented in incident reports.
- [ ] Automated security checks implemented.