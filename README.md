# NetDash by Khudoyberdi Kholbutayev

***Hello and Welcome to my small project***  
***For Advanced usage please use python server if Python is pre‑installed on your device***

```
python -m http.server 5500
# It uses your local Python to host a simple HTTP server on port 5500
```

***Then visit this link***  
`http://localhost:5500/NetDash_by_Kholbutayev.html`

***App provider: Khudoyberdi Kholbutayev***  
***All latency / speed details come from the Cloudflare speed test endpoints***

---

## What JavaScript is used?
- **Vanilla JavaScript (ES6+)** — no frameworks.
- **Fetch API** for network requests.
- **Network Information API** (`navigator.connection`) when available for effective type / downlink / RTT.

## Which libraries are used?
- **Chart.js v4** (via CDN) — renders the latency, download, and upload charts.
  - CDN: `https://cdn.jsdelivr.net/npm/chart.js@4.4.1/dist/chart.umd.min.js`

## External services / endpoints
- **ipify** — public IP (IPv4 / IPv6):
  - `https://api.ipify.org?format=json`
  - `https://api64.ipify.org?format=json`
- **ipapi** — *optional* ISP/ASN & coarse geolocation (only when you toggle “Unlock details”):
  - `https://ipapi.co/json/`
- **Cloudflare Speed Test** — download & upload measurements:
  - Download: `https://speed.cloudflare.com/__down?bytes=<SIZE>`
  - Upload: `https://speed.cloudflare.com/__up` (binary POST)

## Usage
1. Place the HTML file in any folder.
2. **Run a local server** (recommended to avoid browser CORS limits):
   ```bash
   python -m http.server 5500
   ```
3. Open: `http://localhost:5500/NetDash_by_Kholbutayev.html`
4. Click **Start Test**. Toggle **Unlock details** if you want ISP/ASN & location (off by default).
5. **Show Raw** (optional) to view the JSON summary.

## Files
- `NetDash_by_Kholbutayev.html` — single‑file app (privacy‑first build).

## Privacy
- By default, only your **public IP** is fetched.
- ISP/ASN & location are requested **only** if you toggle **Unlock details**.
- This page does **not store** your results.

---

Made with 💙 by **Khudoyberdi Kholbutayev**.
