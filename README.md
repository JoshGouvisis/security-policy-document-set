# Veridian Freight & Logistics: Security Policy Document Set

**Role:** Security Analyst (Simulated, First Security Hire)
**Policy Type:** Foundational GRC Policy Development
**Project:** Portfolio Project 3

> Part of a GRC portfolio series. See also the [NIST CSF Gap Assessment](https://github.com/JoshGouvisis/nist-csf-gap-assessment) and [Third-Party Vendor Risk Assessment](https://github.com/JoshGouvisis/third-party-vendor-risk-assessment), both conducted for a different fictional firm, Meridian Financial Group. Full portfolio: [github.com/JoshGouvisis](https://github.com/JoshGouvisis).

---

## Overview

This project simulates the experience of joining a company as its first dedicated security analyst and building a foundational security policy set from the ground up. The fictional company, Veridian Freight & Logistics, had no formal security documentation when this engagement began. Leadership identified ransomware as a top concern following an incident at a direct competitor, and enterprise clients were increasingly requiring security attestations as a contract condition.

Three policies were developed to establish the foundation: an Acceptable Use Policy governing how employees interact with company systems and data, an Incident Response Policy defining how Veridian detects, responds to, and recovers from security incidents, and an Access Control Policy governing how access to systems and data is granted, maintained, and removed throughout the employee lifecycle. Each policy is aligned to the NIST Cybersecurity Framework 2.0.

---

## About Veridian Freight & Logistics

| Attribute | Detail |
|-----------|--------|
| Employees | ~300 across headquarters and two regional offices |
| Workforce | Hybrid, significant remote population |
| Infrastructure | AWS (cloud), Microsoft 365 (email, collaboration, documents) |
| Applications | Custom logistics tracking web application, SaaS HR, payroll, and CRM platforms |
| Data | Customer PII (names, addresses, contact info), payment card data processed via third-party processor |
| Security Posture at Engagement Start | No security team, no written policies, IT handling security part time |
| Key Risk Driver | Ransomware concern following competitor incident; enterprise clients requiring security attestations |

---

## Policy Documents

| File | Description |
|------|-------------|
| `acceptable-use-policy.md` | Rules governing employee use of Veridian systems, devices, email, data, and personal devices in a hybrid environment |
| `incident-response-policy.md` | Incident definition, severity classification, response lifecycle, escalation paths, and post-incident review requirements |
| `access-control-policy.md` | Full account lifecycle (provisioning, modification, deprovisioning), MFA requirements, privileged access controls, and quarterly access reviews |

---

## NIST CSF 2.0 Mapping

| Policy | NIST CSF Function(s) | Subcategories |
|--------|----------------------|----------------|
| Acceptable Use | Protect | PR.AT-01, PR.AC-01, PR.AC-03, PR.DS-01, PR.DS-05, PR.PS-01 |
| Incident Response | Detect, Respond, Recover | DE.AE-02, DE.AE-03, DE.CM-01, RS.MA-01, RS.MA-02, RS.AN-01, RS.AN-03, RS.MI-01, RS.CO-02, RS.CO-03, RC.RP-01, RC.CO-01 |
| Access Control | Protect | PR.AA-01, PR.AA-02, PR.AA-03, PR.AA-05, PR.AC-01, PR.AC-03, PR.AC-04, PR.AC-07, PR.PS-01 |

The Incident Response Policy intentionally touches the most framework functions, spanning Detect, Respond, and Recover, because effective incident response requires capabilities across all three. The Access Control and Acceptable Use policies are both anchored in the Protect function, reflecting that these are preventive controls designed to reduce the likelihood and impact of an incident before one occurs.

---

## What I Learned

Writing three policies from scratch for the same company back to back taught me something I don't think I could have learned just by reading about policy. The hardest part wasn't writing the rules. It was figuring out why each rule needed to exist for Veridian specifically and making sure every section reflected the actual environment rather than generic language that could belong to any company.

The access control policy was the one that surprised me the most. I went in thinking it was mostly about giving people access to the right systems. What I ended up spending the most time on was deprovisioning and access reviews, the parts that happen after access is granted. That's where the real risk lives, and it's also where I could see most clearly how things go wrong in practice. Someone changes roles and keeps their old access. Someone leaves and their account stays active for weeks. Those aren't hypothetical scenarios, they're the most common access control failures in real organizations.

The incident response policy was the most challenging to write because it had to be specific enough to actually be useful during a real incident while still being a policy and not a technical runbook. Getting the severity tiers right took the most iteration. I kept asking myself whether someone could read a tier description at 2am and quickly determine whether their situation qualified. That became my test for whether the language was clear enough.

The acceptable use policy felt the most straightforward at first, but the BYOD and data handling sections pushed me to think carefully about Veridian's hybrid workforce and the fact that they store customer PII and process payment data. A generic AUP wouldn't cover any of that specifically. Making it feel like it actually belonged to this company, rather than a template, was the goal throughout all three.

---

## Skills Demonstrated

- Security policy development aligned to NIST CSF 2.0
- NIST CSF subcategory mapping
- Incident severity classification and escalation design
- Access control lifecycle management including deprovisioning
- Writing for a business audience in a policy format
- Translating framework requirements into operational controls

---

## About Me

GRC & Security Risk Analyst with 12 years in enterprise risk management, transitioning into GRC and cybersecurity. CompTIA Security+ certified (SY0-701). Google Cybersecurity Professional Certificate. ISC2 CC, Certified in Cybersecurity. CySA+ in progress. Based in Phoenix, AZ.

[LinkedIn](https://www.linkedin.com/in/joshgouvisis/) | [GitHub](https://github.com/JoshGouvisis)
