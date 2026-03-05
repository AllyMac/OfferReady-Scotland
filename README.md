# OfferReady Scotland

A free, browser-based Scottish home buying calculator. Compare properties, calculate LBTT, mortgage repayments and council tax - all in one place.

🔗 **Live site: [offerready.co.uk](https://offerready.co.uk)**

---

## What it does

- Add multiple properties and compare them side by side
- Calculates **LBTT** (Land & Buildings Transaction Tax) with First Time Buyer relief and Additional Dwelling Supplement (ADS)
- Calculates **mortgage repayments** based on offer amount, deposit, Home Report Value, rate and term
- Calculates **council tax** for all 32 Scottish councils across all bands, including Scottish Water charges
- **Comparison table** appears automatically when 2+ offers exist
- **Affordability section** shows monthly cost as a percentage of take-home pay
- **Share button** generates a URL that encodes your full state - share a comparison with anyone
- **Export PDF** generates a clean summary of all properties and offers
- All data saved to localStorage - nothing is ever sent anywhere

---

## Tech

- Single file (`index.html`) - no build process, no dependencies, no framework
- Vanilla HTML, CSS and JavaScript
- [Phosphor Icons](https://phosphoricons.com/) for SVG icons
- [Cormorant Garamond](https://fonts.google.com/specimen/Cormorant+Garamond) + [DM Sans](https://fonts.google.com/specimen/DM+Sans) via Google Fonts
- Deployed on [Netlify](https://netlify.com)

---

## Data sources

| Data | Source | Update frequency |
|---|---|---|
| Council Tax Band D figures | [Scottish Government CTAS](https://www.gov.scot/publications/council-tax-datasets/) | Every April |
| Scottish Water charges | Scottish Water Unmetered Household Charges leaflet | Every April |
| LBTT rates and bands | [Revenue Scotland](https://www.revenue.scot/taxes/lbtt) | Check annually |
| ADS rate | [Revenue Scotland](https://www.revenue.scot/taxes/lbtt/additional-dwelling-supplement) | Check annually |

Current figures: **2025/26**

---

## LBTT rates (correct as of April 2025)

| Band | Rate |
|---|---|
| Up to £145,000 | 0% |
| £145,001 – £250,000 | 2% |
| £250,001 – £325,000 | 5% |
| £325,001 – £750,000 | 10% |
| Over £750,000 | 12% |

First Time Buyer relief raises the 0% band to £175,000 (max saving £600).
Additional Dwelling Supplement (ADS): **8%** on full purchase price (from December 2024).

---

## Updating council tax figures (each April)

1. Download the latest CTAS dataset from `gov.scot/publications/council-tax-datasets/`
2. Update the `COUNCILS` object in `index.html` with the new Band D figures
3. Download the new Scottish Water Unmetered Household Charges leaflet
4. Update the `SW_WATER` and `SW_SEWERAGE` objects in `index.html`
5. Update the footer year reference

---

## Deploying

Netlify deploys automatically on every push to `main`. To deploy manually, drag the project folder to [netlify.com](https://netlify.com).

---

## Disclaimer

For guidance only - not financial or legal advice. Always verify figures with your solicitor, mortgage broker and local council.
