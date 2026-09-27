# Phone Finder

Phone Finder ala GSMArena dalam **single HTML**. Deploy langsung ke Vercel.

## Deploy
1. Push repo ini
2. https://vercel.com/new → import repo `finder` → Framework: **Other** → Deploy

## Fitur
- Filter: Brand, Year (slider min-max), Availability, Price EUR (slider), 2G/3G/4G/5G, Dual SIM
- Search nama HP
- 10.506 HP, tahun 1994–2021
- Gambar hotlink dari CDN GSMArena (fdn2.gsmarena.com), ada fallback "No Image"

## Catatan
- Dataset sumber: github.com/foykes/gsm-arena-dataset (terakhir update 2021,
  jadi HP 2022–2026 belum ada)
- Data statis embedded di index.html — tanpa backend, tanpa CORS issue

## Update Data
Scrape ulang pakai scraper dari dataset sumber, proses jadi format array,
ganti `const DATA = [...]` di index.html.
