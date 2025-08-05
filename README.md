# 🛡️ Zero Trust Architecture – Scalable Enterprise Network Implementation

## 🧠 Overview
This project provides a practical implementation of **Zero Trust Architecture (ZTA)** on a scaled-down enterprise network using **Cloudflare Access**, **Tailscale**, and **OKTA**. It simulates a real-world environment where a company (@Spiral) seeks to secure a web-based application and remote user access under Zero Trust principles — eliminating implicit trust and enforcing least privilege policies.

## 🎯 Objective
To move beyond the theoretical definitions of Zero Trust and:
- Design a **functional solution** with industry tools.
- Implement **scalable policy controls** for session security, app whitelisting/blacklisting, and device identity verification.
- Provide **clear documentation** for reproducibility and education.

## 🧰 Tools & Technologies Used
- **Cloudflare Access** – Application gateway and policy engine
- **Tailscale** – Secure VPN mesh and device identity management
- **OKTA** – Identity Provider (IdP) for access authentication
- **Linux CLI / bash** – Configuration, device management
- **YAML / JSON** – Policy definition formats
- **Markdown / Diagrams.net** – Documentation and architecture diagrams

## 🔧 Implementation Highlights
- Built a **software-defined perimeter (SDP)** protecting @Spiral’s internal web-based app.
- Defined access policies based on:
  - Device trust
  - User identity
  - Geo/IP-based restrictions
  - Time-based access windows
- Configured **remote access gateway** for @Spiral employees via Tailscale
- Integrated **OKTA SSO** with Cloudflare Access for centralized authentication
- Enabled @Spiral's security team to:
  - Whitelist/blacklist applications and URLs
  - Add/remove employee devices
  - Set granular per-session access levels

## ⚠️ Challenges Faced
- **Gap between concept and implementation**: At the time of the research, few practical Zero Trust deployments were publicly documented.
- Leading me to manually **translate abstract Zero Trust principles** into enforceable technical policies.
- Created detailed internal documentation to map **business requirements** (least privilege, secure remote access) into:
  - Technical toolchain configuration
  - Logical security zones
  - Identity & device controls

## 📄 Documentation Included
- ✅ Zero Trust Concept Guide (What it is, Why it matters)
- ✅ Setup Instructions for Cloudflare, OKTA, and Tailscale integration
- ✅ Policy and rule design for Zero Trust controls
- ✅ Architecture diagrams showing session flow and access zones

## 🔐 Security Concepts Demonstrated
- Zero Trust Architecture (ZTA)
- Identity-Centric Access Control
- Least Privilege Enforcement
- Secure Remote Access
- Micro-Segmentation

## 📈 Outcomes
- Successfully deployed a simulated ZTA model that is scalable to an enterprise use case
- Documented solution adaptable to other networks
- Delivered a research-backed playbook for small to mid-sized orgs exploring ZT adoption

## 🖼️ Visuals
> <img width="596" height="375" alt="image" src="https://github.com/user-attachments/assets/eb41c8fd-fe7a-4d9c-b199-a9e7d7f8126f" />

> <img width="674" height="387" alt="image" src="https://github.com/user-attachments/assets/a2451a55-2a3f-471e-a5f0-0fbf52022ffd" />



---

---

## 🧩 Future Enhancements
- Integrate threat detection using Cloudflare logs + SIEM
- Build dynamic device attestation policies
- Expand to multi-region policy enforcement
