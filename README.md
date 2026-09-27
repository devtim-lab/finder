# 🔍 Repo Finder

Single HTML untuk mencari repository GitHub. Deploy langsung ke Vercel.

## Deploy ke Vercel
1. Push repo ini
2. Buka [vercel.com/new](https://vercel.com/new) → import repo `finder`
3. Framework: **Other** → Deploy
4. Selesai, dapat URL `https://finder-xxx.vercel.app`

Atau via Vercel CLI:
```bash
vercel --prod
```

## Fitur
- Cari repository berdasarkan kata kunci
- Filter bahasa pemrograman
- Urutkan: stars / forks / update terbaru
- Load more (pagination)
- Tanpa backend, langsung pakai GitHub Search API (CORS sudah terbuka)

## Catatan Rate Limit
- Tanpa token: **10 request search/menit**
- Kalau mau lebih longgar, tambahkan GitHub token di header (opsional)
