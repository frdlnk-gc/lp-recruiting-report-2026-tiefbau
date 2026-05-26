# lp-recruiting-report-2026-tiefbau

Landingpage für den GreenCareers Recruiting-Report 2026 — **Straßen- und Tiefbau Edition**.

**Live:** https://recruiting-report-2026-tiefbau.green-careers.de/
(nach DNS-Setup bei IONOS — analog zur GaLaBau-LP)

## Inhalt

| Datei | Zweck |
|---|---|
| `index.html` | Landingpage mit Formular → schickt Lead per WhatsApp + E-Mail |
| `Download-Seite/index.html` | Bestätigungs-/Download-Seite + Termin-Anfrage-Formular |
| `recruiting-report-2026-tiefbau.pdf` | 32-Seiten Report (Anthrazit/Orange, Tiefbau-spezifisch) |
| `hero-images/hero-tiefbau-web.jpg` | Hero-Foto (Liebherr-Bagger + Asphaltwalze + Bauleiter) |
| `logo-*.png` / `favicon-*.png` | GreenCareers Brand Assets |
| `CNAME` | Custom Domain für GitHub Pages |

## Make-Webhooks

In beiden HTML-Dateien sind die Webhook-URLs aktuell auf den **GaLaBau-Webhooks** (Platzhalter). Diese müssen durch die **neuen Tiefbau-Webhooks** ersetzt werden:

- `index.html` → Variable `MAKE_WEBHOOK_URL` (LP-Formular → Report-Versand WhatsApp)
- `Download-Seite/index.html` → Variable `TERMIN_WEBHOOK_URL` (Termin-Anfrage)

Beide schicken `source: 'lp-recruiting-report-2026-tiefbau'` bzw. `'download-page-termin-anfrage-tiefbau'` mit — damit kann Make sauber filtern.
