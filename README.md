# NominaGuard Analytics
**Tagline:** *Predict, Protect, and Secure Your Digital Identity.*

## 1. Product Overview
**NominaGuard Analytics** is a predictive cybersecurity and digital reputation platform that calculates an individual's vulnerability to personal domain squatting, impersonation, and digital extortion. 

Using Open Source Intelligence (OSINT) and our proprietary **Personal Domain Risk Matrix (PDRM)**, the platform analyzes an individual's profession, geographic legal jurisdiction, career stage, visibility, and gender to generate a highly accurate **Vulnerability Score (1-100)**. 

Our mission is to shift personal domain protection from a reactive, high-cost legal nightmare ($5,000+ per legal dispute) into a proactive, low-cost automated insurance policy ($20/year).

**Target Audience:**
*   **B2C (Direct to Consumer):** High-net-worth individuals, doctors, lawyers, public figures, creatives, and rising professionals.
*   **B2B2C (Enterprise/Institutional):** Professional regulatory bodies (e.g., Law Societies, Medical Councils), Universities (graduating classes), Wealth Management firms, and Talent Agencies.

---

## 2. Interactive Single Page Web App (SPA) Calculator
The entry point for NominaGuard Analytics is a lightweight, high-conversion Single Page Application (SPA) designed to act as a lead-generation tool and instant risk assessor.

**How the SPA Works:**
*   **User Inputs:** A clean, multi-step UI collects the following data points:
    *   **First & Last Name:** (To query TLD availability in the background).
    *   **Profession/Industry:** (Dropdown classifying fields by wealth/public visibility. e.g., "Medical Professional", "Legal", "Executive", "Creative").
    *   **Age Bracket & Career Stage:** (e.g., "Student", "Mid-Career", "Senior/Partner").
    *   **Jurisdiction:** (e.g., IE, UK, EU, US, CA - used to calculate legal recovery difficulty).
*   **Calculation Logic:** The React/Vue.js frontend passes data to our PDRM API. The algorithm applies risk multipliers (e.g., +20% for high-wealth professions, +15% for jurisdictions with weak personal name protections like the US/UK).
*   **Output Visualization:** 
    *   Displays a dynamic "Speedometer" or "Risk Gauge" (e.g., **Risk Score: 87/100 - CRITICAL**).
    *   Generates a personalized brief explaining *why* the score is high (e.g., *"As a medical professional in the UK, your name is subject to public directory scraping, and Nominet DRS provides limited protection for personal names."*).
    *   Includes a real-time availability check for their exact `.com`, `.ie`, `.co.uk`, etc.

---

## 3. Core Features (MVP Launch)

*   **The PDRM Scoring Engine:** The backend intelligence driving the SPA, processing live TLD availability alongside demographic vulnerabilities.
*   **Global TLD & Attack Vector Scanner:** Instantly scans over 1,500 TLDs. Categorizes threats into: *Exact Matches* (FirstLast.com), *Professional Signifiers* (DrFirstLast.ie), *Typosquatting* (FirstLats.com), and *Attack Vectors* (FirstLastScam.com).
*   **ROI / Cost-to-Recover Calculator:** A localized financial projection feature. Displays a side-by-side comparison: *"Cost to secure today: €25. Estimated cost to litigate in Ireland (IEDR via WIPO) if stolen: €4,500."*
*   **Public Registry Vulnerability Alerts:** Monitors professional databases (e.g., Medical Council registers, Bar Association admissions). Flags when an individual's visibility spikes, indicating automated bots are likely targeting them.
*   **One-Click Defensive Registration:** Integrated domain registrar API (e.g., via Namecheap or GoDaddy). Users can instantly purchase and "park" their highest-risk domains directly from the NominaGuard dashboard.

---

## 4. Product Roadmap

### Phase 1: Deep Perimeter Defense (Q3 2026 - Q4 2026)
*   **Social Handle Syncing API:** Integration to check if the exact domain match is also available across X, LinkedIn, Instagram, and TikTok, allowing users to secure a unified digital perimeter.
*   **"Family Vault" Accounts:** Allows parents to create profiles, monitor the risk matrix for their children, purchase domains at birth, and track their risk as they grow.

### Phase 2: Enterprise & Guild Integrations (Q1 2027 - Q2 2027)
*   **University Alumni Portal:** A white-label B2B widget for Universities. Upon graduation, students receive a secure "NominaGuard Scan" and their primary professional domain for one year.
*   **HR / Executive Onboarding API:** Integration for corporate HR platforms. When a new C-suite executive is hired, the system automatically checks and secures their personal domains to mitigate Business Email Compromise (BEC) attacks.

### Phase 3: Active Threat Intelligence (Q3 2027 - Q4 2027)
*   **Dark Web & Impersonation Monitoring:** If a user's domain is already squatted, this feature continuously monitors the domain for MX Record changes (indicating email server setup for impersonation) or malicious hosting drops.
*   **AI Predictive Typosquatting:** Machine learning models that predict the most likely misspellings a malicious actor will buy based on the user's regional dialect and keyboard layouts (e.g., QWERTY vs. AZERTY).

### Phase 4: Automated Legal Remediation (2028 and beyond)
*   **AI-Generated Cease & Desist (C&D):** An automated tool that utilizes regional laws (e.g., GDPR, US ACPA) to generate and dispatch legal notices to registrars and squatters.
*   **Dispute Packet Generator:** Auto-generates the foundational framework and evidence logs for a UDRP, IEDR, or Nominet complaint, saving users thousands in initial legal drafting fees.
