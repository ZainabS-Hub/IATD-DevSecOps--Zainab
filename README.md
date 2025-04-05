# IATD-DevSecOps
Vulnerable application for DevSecOps Microcredential

The repository was cloned from [https://github.com/erev0s/VAmPI](https://github.com/erev0s/VAmPI)
## 🔍 ZAP DAST Scan (Dynamic Application Security Testing)

Automated ZAP scans are run on every push using GitHub Actions. The pipeline runs OWASP ZAP against the [VAmPI](https://github.com/erev0s/VAmPI) API and produces security reports.

![ZAP CI Status](https://github.com/zainabs-hub/IATD-DevSecOps/actions/workflows/ci-pipeline.yml/badge.svg)

🔗 [View latest pipeline run](https://github.com/zainabs-hub/IATD-DevSecOps/actions)  
📥 [Download ZAP Report Artifact](https://github.com/zainabs-hub/IATD-DevSecOps/actions) *(Reports available under "Artifacts")*

> **Includes:**  
> - `report_html.html` – human-readable visual report  
> - `report_md.md` – markdown version  
> - `report_json.json` – for API integration

---

## 📦 Project Setup

```bash
# Clone the repository
git clone https://github.com/zainabs-hub/IATD-DevSecOps.git
cd IATD-DevSecOps

# Launch vulnerable API (optional)
docker-compose up -d