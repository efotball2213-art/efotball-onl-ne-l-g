# eFootball Altın Lig

eFootball ligimiz için karanlık tema ve altın tonlarında tasarlanmış canlı lig sitesi.

- **Ana sayfa (`/`)** — kupa görselli giriş bölümü, lider ve gol kralı kartları, istatistik şeridi, canlı puan tablosu (sıralama değişince satırlar kayarak yer değiştirir), gol krallığı kürsüsü ve son maçlar.
- **Admin paneli (`/admin`)** — şifreyle korunur. Takım ekleme/düzenleme, puan tablosunu elle ayarlama (G/B/M, atılan/yenen, puan düzeltmesi, form), maç sonucu girme (istatistikler otomatik güncellenir, geri alınabilir), gol krallığında +/− ile gol/asist güncelleme, lig adı/sezon/duyuru ayarları ve sezon sıfırlama.
- **Canlı güncelleme** — site birkaç saniyede bir değişiklik olup olmadığını kontrol eder; admin bir şey kaydettiğinde tüm ziyaretçilerde tablo anında güncellenir, değişen satırlar parlar, yeni maçta düdük + gol sesi ve konfeti çıkar.
- **Ses efektleri** — Web Audio ile üretilir (düdük, gol/tribün, altın çınlama, tıklama). Sağ üstteki hoparlör ikonundan kapatılabilir.

## Teknolojiler

TanStack Start (React 19), Tailwind CSS 4, Netlify Database (Postgres) + Drizzle ORM, Netlify Image CDN, Netlify'da barındırma.

## Yerel çalıştırma

```bash
pnpm install
netlify dev
```

## Admin şifresi

Varsayılan şifre kodda tanımlıdır. Değiştirmek için Netlify'da `ADMIN_PASSWORD` ortam değişkenini ayarlayın (isteğe bağlı olarak oturum imzalama anahtarı için `ADMIN_SECRET`).
