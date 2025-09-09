# 🛡️ TrustShield Sentinel

**Privacy-first Insider Threat Detection for Wema Bank Hackathon (Challenge Five)**

---

## 🌍 Overview

Insider threats are one of the toughest challenges in banking. 
- Some employees may **accidentally** expose data.  
- Others may **intentionally** misuse their access.  
- Traditional monitoring tools often feel like *“Big Brother”*, creating mistrust and harming workplace culture.  

**TrustShield Sentinel** solves this by detecting unusual staff activity with **simple behavioral signals** (not surveillance) and engaging employees with **friendly nudges** instead of accusations.  

Employees become **partners in security**, not suspects.

---

## 🎯 Problem Statement

How might we detect and contain insider threats in Wema Bank **while preserving employee trust and respecting privacy**?

---

## 💡 Our Solution

**TrustShield Sentinel** monitors *patterns, not people*.  

- ✅ Detects unusual logins, device use, or file activity.  
- ✅ Sends **supportive prompts** to staff:  
  > “We noticed some unusual activity. Was this expected?”  
- ✅ Preserves privacy by anonymizing data until a credible risk emerges.  
- ✅ Provides a **dashboard for security teams** with risk signals (low/med/high) without naming employees unless escalation is needed.  

---

## 🔎 How It Works

1. **Detection (Backend)**  
   - Define role baselines (e.g., teller vs. HR).  
   - Flag anomalies like:  
     - Login after 10 pm.  
     - Bulk file downloads.  
     - New device or location.  

2. **Engagement (Frontend)**  
   - Employees receive **nudges** through modal popups or chatbot prompts.  
   - Options:  
     - ✅ Yes, this was me  
     - 🚩 No, escalate  
     - 💬 Need help  

3. **Privacy Safeguards**  
   - Only metadata (time, count, location) — no content.  
   - Employee IDs are hashed/anonymized in dashboard.  
   - Alerts auto-expire to prevent over-monitoring.  

4. **Security Dashboard**  
   - Shows anonymized risk alerts.  
   - Risk heatmap or cards by level.  
   - Drill-down only after multiple anomalies.  

---

## 🏗️ Tech Stack

- **Frontend:** React (dashboard + employee modals)  
- **Backend:** Node.js (Express) with mock MongoDB/JSON data  
- **Prototype Data:** Sample employee logs with login times, devices, actions  
 

---

## 🚀 Hackathon MVP Scope

- [ ] Simple anomaly rules engine (3–4 rules).  
- [ ] Mock employee activity logs (10–15 users).  
- [ ] Frontend dashboard with anonymized alerts.  
- [ ] Modal/chatbot flow for employee confirmation.  
- [ ] Pitch deck with story, benefits, and future potential.  

---


---

## 🔮 Future Potential

- Expand from simple rules → AI anomaly detection.  
- Integrate with IAM tools (Okta, Azure AD).  
- Add gamified trust scores to build a security culture.  
- Deploy as SaaS for banks & enterprises.  

---

## 📜 License

MIT License (for hackathon demo purposes).
