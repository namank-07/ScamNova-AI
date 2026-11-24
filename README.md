# SCAMNOVA AI

A bilingual (English/Hindi), local-first scam and phishing awareness MVP built with React, TypeScript, Vite, Tailwind CSS, Lucide icons, jsQR and Tesseract.js.

## Run locally
1. Install Node.js 18+.
2. Open this folder in VS Code.
3. Run `npm install`.
4. Run `npm run dev`.
5. Open the local URL printed by Vite.

## Features
- Dark and light themes, remembered in localStorage.
- English/Hindi language selector, remembered in localStorage.
- Message, URL and job/internship analysis with explainable 0–100 scoring.
- URL X-Ray parses URL strings only; it never opens or fetches submitted URLs.
- QR image decoding in-browser with jsQR.
- Screenshot text extraction in-browser with Tesseract.js (English and Hindi language data).
- Scam DNA fingerprint derived deterministically from matched rule labels.
- Local incident report form.
- Nova safety assistant with bilingual rule-based answers (not a live AI model).
- Side-by-side scam message comparison.
- Cyber IQ quiz, scam library, and local scan history.
- Indian cybercrime reporting information (1930 and cybercrime.gov.in).

## Privacy and limitations
Submitted messages and decoded QR contents are not sent to an analysis API. QR destinations are never opened. OCR runs in the browser; Tesseract.js may download language model assets when first used. The user should review OCR output for errors.

The detector is an awareness tool, not a guarantee of safety. It uses known text and URL patterns, may produce false positives, and can miss new or contextual scams. Threat DNA scores are rule-match strengths, not probabilities. Incident reports and history are stored in browser localStorage and remain on that device unless browser data is cleared.
