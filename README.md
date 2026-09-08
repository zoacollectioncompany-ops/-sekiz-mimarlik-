# Sekiz Mimarlık — Web Sitesi

Tek dosyalık, statik HTML site. Build adımı yok, herhangi bir statik hosting'e (GitHub Pages, Vercel, Netlify) doğrudan yüklenebilir.

## GitHub Pages ile Yayınlama

1. GitHub'da yeni bir repository oluştur (örn. `sekiz-mimarlik-web`).
2. Bu repodaki `index.html` dosyasını reponun **kök dizinine** yükle (sürükle-bırak ile veya `git push`).
3. Repo → **Settings → Pages** sekmesine git.
4. **Branch** olarak `main` (veya `master`) ve klasör olarak `/root` seç, **Save**'e bas.
5. 1-2 dakika içinde site şu adreste yayına girer:
   `https://<kullanıcı-adın>.github.io/<repo-adı>/`

### Kendi alan adını bağlamak istersen
1. Repo köküne içeriği alan adın olan bir `CNAME` dosyası ekle (örn. `sekizmimarlik.com`).
2. Alan adı sağlayıcında bir `CNAME` (veya `A`) kaydını GitHub Pages IP/host'una yönlendir.
3. Settings → Pages → Custom domain kısmına alan adını gir ve HTTPS'i etkinleştir.

## Git ile hızlı yükleme (terminalden)

```bash
git init
git add index.html README.md
git commit -m "Sekiz Mimarlık web sitesi"
git branch -M main
git remote add origin https://github.com/<kullanici-adin>/<repo-adi>.git
git push -u origin main
```

Ardından yukarıdaki 3-4. adımlarla Pages'i aktive et.

## Notlar
- Fontlar (Fraunces, Manrope) Google Fonts CDN üzerinden yükleniyor — internet bağlantısı gerektirir.
- WhatsApp ve arama butonları `+90 532 548 63 04` numarasına sabitlenmiştir; numarayı değiştirmek için dosya içinde `905325486304` ifadesini ara-değiştir yap.
- Form/teklif modülü yok; iletişim tamamen "Hemen Ara" ve "WhatsApp'tan Yaz" butonları üzerinden yürüyor.
