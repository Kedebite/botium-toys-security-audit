# Internal Security Audit — Botium Toys

## Overview
This project is a full internal security audit conducted for Botium Toys, a fictional mid-size retailer with both physical stores and an e-commerce platform. It demonstrates the ability to assess an organization's security posture across multiple domains, identify and prioritize risk, and communicate findings in a professional audit report suitable for a leadership or compliance audience.

## Objective
Evaluate Botium Toys' security controls across physical security, network architecture, access control, data protection, patch management, security awareness, and incident response — then deliver a risk-rated findings report with prioritized, actionable recommendations.

## Methodology
Findings were developed through a controls-based review, mapping observed practices in each domain against baseline expectations drawn from the **NIST Cybersecurity Framework** (Identify, Protect, Detect, Respond, Recover) and **PCI DSS** requirements relevant to a business handling card payment data. Each identified gap was assigned a risk level — High, Medium, or Low — based on likelihood of exploitation and potential business impact.

## Key Findings
The audit identified **4 High-risk**, **3 Medium-risk** gaps across 8 control domains, including:

| Domain | Gap | Risk |
|---|---|---|
| Access Control / IAM | Shared local admin credentials, no individual accountability | High |
| Network Security | Flat, unsegmented network — POS shares a VLAN with guest Wi-Fi | High |
| Password Policy | Vendor-default credentials still in active use on some systems | High |
| Incident Response | No documented plan, roles, or escalation path | High |
| Physical Security | Server closet unmonitored, accessible to any staff member | High |
| Data Protection | Backups unencrypted and stored on-site with production data | Medium |
| Patch Management | No formal patch cadence or verification process | Medium |
| Security Awareness | No training on phishing or incident reporting | Medium |

## Deliverable
The full audit report — including the complete findings table, a 7-item prioritized recommendations table mapped to each risk domain, and a written executive summary and conclusion — is included in this repository:

📄 [**Botium_Toys_Security_Audit.docx**](./Botium_Toys_Security_Audit.docx)

## Top Priority Recommendations
1. **Eliminate shared/default credentials** — enforce individual accounts with password complexity and rotation policy.
2. **Segment the network** — isolate POS/payment systems onto a dedicated VLAN, separate from staff and guest traffic.
3. **Restrict physical access** to the server closet with badge access and basic camera coverage.

(Full list of 7 prioritized recommendations, with expected outcomes, is in the report.)

## Skills Demonstrated
- Security risk assessment and audit methodology
- Mapping findings to industry frameworks (NIST CSF, PCI DSS)
- Risk prioritization (likelihood × impact)
- Professional security documentation and report writing for a non-technical/leadership audience

## Status
Complete
