# Amani Consulting Group — Corporate website

A responsive, bilingual (EN/FR) **static website** for Amani Consulting Group. No WordPress, database, PHP runtime, Node server or build tool is required.

## Deploy on Vercel

1. Upload `index.html`, `styles.css`, `script.js`, `favicon.svg`, and `vercel.json` to the **root** of the `amaniconsulting-source/amani-consulting-website` repository.
2. In Vercel, import that repository into the existing Pro team.
3. Select **Framework Preset: Other**; keep Root Directory `./`. Leave Build Command blank. If Vercel asks for an Output Directory, use `.` for this root-level static site.
4. Deploy and verify the `.vercel.app` preview on desktop and mobile, including both languages and links.
5. Add `amaniconsultinggroup.com` and `www.amaniconsultinggroup.com` in Project Settings > Domains.
6. At Arvixe DNS, update only website records to values **actually shown by Vercel**. Preserve MX, SPF, DKIM, DMARC and nameservers to avoid breaking email.
7. Switch DNS only after review; retain Arvixe hosting/email until everything is verified.

## Important pre-publication review

- **Brand:** Header uses a simplified vector interpretation of the Amani symbol as a temporary placeholder; replace with the approved original logo asset.
- **Case studies:** Confirm final wording and publication rights for each DRC client/project. US retail clients are intentionally unnamed.
- **DaatLayer:** Presented as a product initiative; avoid implying unverified customer results.
- **Offline sites:** PosteMarket is intentionally not linked. Check public availability before linking CodePostal.
- **Contact:** Email uses `mailto:` (no external form provider). Verify that the Arvixe-hosted mailbox stays active or migrate email separately.
- **Fonts:** Google Fonts are loaded online; replace with local font files for an entirely self-contained site, if desired.

## Local preview

Run `python -m http.server 8000` in the project directory, then visit `http://localhost:8000`.
