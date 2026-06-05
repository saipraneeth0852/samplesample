# Structured Data Capture Workspace for LC-Driven Invoice Generation

🚀 **Live Site:** [Structured Data Capture Workspace](https://saipraneeth0852.github.io/samplesample/)

An interactive workspace designed for exporters to perform structured data capture for commercial invoices aligned with **SWIFT MT700** and **ICC UCP 600** specifications. It ensures data symmetry between internal export documentation pipelines and downstream letter of credit structures.

---

## 🔍 Key Compliance Features
- **MT700 Engine Alignment**: Structured data inputs mapped to specific SWIFT MT700 field tags (e.g. `[MT59]`, `[MT50]`, `[MT57/54]`, `[31D]`, `[44E/C/B]`, `[43P/T]`, `[45A]`).
- **Real-Time Validation Engine**:
  - Expiry date verification against shipment date rules.
  - Geographical structure checks for expiry places (ISBP 821 alignment).
  - Normalization suggestions for applicable rules (`UCP 600 ICC Publication No. 600`).
  - Out-of-country bank charge allocation validation (UCP 600 Art. 37).
  - HS Code formatting verification (standard 8-digit tariff code check).
- **Logistics Integrity Controls**: Handles Incoterms rules, shipment locations, partial shipments, and transshipment flag alerts.
- **Dynamic Valuation Matrix**: Automatic calculations for Base FOB Value, Freight, 110% Insurance Protection, and Total CIF Valuation.
- **Commercial Documents Builder**: Interactive checklist to compile mandatory export documentation (e.g., Commercial Invoice, Packing List, Certificate of Origin, Insurance Policy, etc.).

---

## 🛠 Tech Stack
- **Frontend**: Standard-compliant HTML5, CSS3 Custom Properties (CSS variables), Vanilla JavaScript.
- **Styling**: Sleek slate-dark theme design system with custom HSL variables, responsive grid configurations, dynamic status flags, and custom components.
- **Hosting**: Automatically deployed to **GitHub Pages** via GitHub Actions.

---

## 📂 Deployment Configuration
This workspace is set up to automatically deploy to GitHub Pages on every push to the `main` branch. 
The workflow file can be found in [.github/workflows/deploy.yml](.github/workflows/deploy.yml).
