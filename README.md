# Awesome-Fraud-Detection-Prevention

# Top Fraud Detection & Prevention Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on E-commerce Chargeback Protection, Transaction Risk Scoring & Self-Hosted Fraud Engines*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Fraud Detection & Prevention**. These tools enable merchants and fintechs to identify risky transactions, block fraudulent orders, reduce chargebacks, and approve legitimate customers—balancing loss prevention with conversion rate optimization.

**Examples** include Shopify Fraud Analysis, Signifyd, Riskified, Sift, SEON, Forter, Kount, NoFraud, ClearSale, and FraudLabs Pro (the category leaders).

**Open-source emphasis**: Fraud Detection is a domain where open-source tooling is **emerging but still catching up to commercial SaaS**. The strongest active projects are **Marble (CheckMarble)**, a real-time transaction monitoring and AML decision engine positioned as an open-source alternative to Feedzai, SEON, and SumSub, with 475 GitHub stars and a Go backend , and **Jube**, an AGPL-3.0 licensed AML/fraud platform with adaptive ML and a rule engine . Other projects like **FraudGuard** provide a security framework for threat detection and abuse monitoring . However, no open-source project matches the **global merchant network intelligence** of Signifyd or Riskified—those rely on cross-merchant data from billions of transactions that a self-hosted tool cannot replicate.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Shopify Fraud Analysis](https://help.shopify.com/en/manual/orders/fraud-analysis)**  
  Shopify's native fraud detection tool that flags high-risk orders using indicators like mismatched billing/shipping addresses, suspicious IPs, and multiple failed payment attempts; provides recommendations (cancel, investigate, or fulfill) directly in the admin.

- **[Signifyd](https://www.signifyd.com/)**  
  Enterprise fraud protection platform with a **financial guarantee** on approved orders; Winter 2026 release adds **Account Integrity** (protecting sign-up/login before checkout), **Selective Appeasements** (stopping refund fraud), and an embedded Shopify app for reviewing orders without leaving admin . Pioneering **Agentic Commerce** protection for AI-agent-initiated transactions .

- **[Riskified](https://www.riskified.com/)**  
  Chargeback protection and fraud prevention platform with a **global Merchant Network** covering over a billion historical transactions; uses **Smart Linking** to identify individuals behind online interactions and **Decision Optimizer** to generate real-time decisions . Provides guaranteed approvals and explainable machine learning .

- **[Sift](https://sift.com/)**  
  AI-powered fraud platform with **AI Agents** for fraud teams: **Attack Detection/Investigation/Response Agents** for attack defense, **Review Agent** for case review with readable reasoning, and **Risk Activity Agent** for behavioral history analysis . Includes an **MCP Server** for querying Sift directly from AI tools . Sift Score and Workflows act on events in **under 150ms** .

- **[SEON](https://seon.io/)**  
  Fraud prevention and AML compliance platform integrating **900+ data signals** (digital footprint, device intelligence, behavioral biometrics, AI agent detection) . Covers pre-onboarding risk analysis, identity verification, transaction monitoring, and case management with AI-assisted investigations and SAR narrative generation .

- **[Forter](https://www.forter.com/)**  
  AI platform for fraud and payments with **1.8 billion identities** across its merchant network . Focused on **Agentic Commerce** infrastructure: **Agentic Orchestration** for supporting AI-agent transactions, **Trusted Agentic Commerce Protocol**, and an **Agentic Activity dashboard** for visibility into AI-driven traffic . Includes **Forter Prism**, an in-portal AI copilot for investigations .

- **[Kount](https://www.kount.com/)**  
  Fraud prevention and chargeback management platform (now part of Equifax); June 2026 release adds **AND/OR logic for Linked Analysis** in case investigations, improved chargeback prevention alert resolutions, and UI updates for prevention alerts table .

- **[NoFraud](https://www.nofraud.com/)**  
  Shopify-focused fraud prevention app with a **4.8 rating** (163 reviews); users report "zero chargebacks" and seamless integration, with a guarantee that covers fraudulent orders . Praised for protecting revenue without blocking legitimate customers.

- **[ClearSale](https://www.clear.sale/)**  
  Brazilian fraud prevention platform with **20+ years of market experience**; combines statistical models, machine learning, and behavioral analysis with **manual review by trained specialists** for complex transactions . Focuses on transparency in approval decisions and reducing false declines for small/mid-size e-commerce .

- **[FraudLabs Pro](https://www.fraudlabspro.com/)**  
  Fraud detection API with SDKs including **Go SDK** for transaction analysis, fraud scoring based on IP/email/billing/shipping, **credit card issuing bank validation**, and **SMS verification** . Provides a free tier for developers.

## Open-Source GitHub Projects

### Transaction Monitoring & Decision Engines

- **[Marble (CheckMarble)](https://github.com/checkmarble/marble)**  
  The strongest open-source **real-time fraud and AML decision engine** available (475 GitHub stars, Go/React, open core) . Positioned as an open-source alternative to Feedzai, SEON, and SumSub. Features **real-time or post-trade transaction monitoring** with a custom data model that mirrors your data warehouse, customer/company screening against sanctions/PEP/adverse media, unified case manager, AI automation for rule building, embedded analytics, unalterable audit trail, RBAC/SSO, and SOC 2 Type II (cloud version) . Self-hosted open-source core is free; licensed version adds advanced features . **The best starting point for organizations building a self-hosted fraud/AML monitoring system.**

- **[Jube](https://github.com/jube-home/aml-fraud-transaction-monitoring)**  
  Open-source **AML and fraud detection platform** with real-time transaction monitoring and **adaptive ML** (supervised + unsupervised, neural network topology search) combined with a rule engine (58 GitHub stars, C#/.NET, AGPL-3.0) . Provides a complete platform for real-time monitoring with machine learning capabilities. **Strong for teams wanting ML-driven fraud detection** with a permissive (AGPL) license, though it is smaller and less documented than Marble.

### Security Frameworks & Abuse Monitoring

- **[FraudGuard](https://github.com/fraudguard/fraudguard)**  
  Open-source security framework for **threat detection, fraud prevention, and abuse monitoring** (1,552 GitHub stars, AGPL-3.0) . Self-hosted solution with a built-in dashboard and risk scoring. **Broader than e-commerce fraud**—covers abuse monitoring across products, useful for platforms needing to detect fraudulent signups, abuse patterns, and security threats alongside payment fraud.

### Additional Strong Open-Source Options

- **OpenSanctions + Yente** — Open database of sanctions, PEPs, and persons of interest (320+ sources); Yente provides a self-hosted screening API with Docker and ElasticSearch backend . **Essential for sanctions/PEP screening** as part of a broader fraud/AML stack, though commercial data licensing may be required .
- **Watchman (moov-io)** — Open-source sanctions list screening tool (Apache 2.0) with Jaro-Winkler distance scoring, auto-refresh of government lists, Docker deployment, and zero external dependencies . **Directly replaces the sanctions-screening portion** of commercial fraud platforms.
- **No mature open-source equivalent to Signifyd or Riskified exists** — The **cross-merchant network intelligence** (billions of transactions from thousands of merchants) that powers Signifyd and Riskified's decisions is fundamentally not replicable by a self-hosted tool. Open-source fraud engines rely on your own transaction data, not a global network.

**Frameworks for building custom systems**: **Marble** provides the most complete open-source foundation for real-time transaction monitoring and case management . **Jube** adds ML-driven detection for teams wanting adaptive models . **FraudGuard** covers broader abuse monitoring beyond payments . For sanctions/PEP screening, combine **Watchman** or **OpenSanctions/Yente** with Marble . No open-source project replicates the network effect of Signifyd or Riskified—expect to rely on your own data and rules.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Fraud detection platforms handling transaction and personal data must comply with applicable privacy regulations (GDPR, CCPA) and payment card industry requirements; **false positives can lose legitimate customers**, and false negatives create chargeback losses. Tuning thresholds requires ongoing monitoring.
- **Open-source fraud detection is strongest for transaction monitoring and AML**—Marble and Jube provide production-ready decision engines , and Watchman/OpenSanctions cover sanctions screening . However, **no open-source project replicates the cross-merchant network intelligence** of Signifyd, Riskified, or Forter, which derive signal from billions of transactions across thousands of merchants. Organizations requiring network-effect fraud protection should evaluate commercial platforms.
- Verify license terms for commercial use; Marble uses an open-core model (core open-source, advanced features licensed) , Jube uses AGPL-3.0 , and FraudGuard uses AGPL-3.0 .

---

**Made for e-commerce merchants, risk analysts, payment engineers, and fraud operations teams.**  
Let's make fraud detection more open, but with clear eyes about the network-effect moat that commercial platforms hold.
