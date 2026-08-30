# YKS 2027 • Akıllı Koç PWA v3

GitHub Pages üzerinden tablet ve telefonlarda kullanılmak üzere hazırlanmış, verileri cihazda tutan tek sayfalı PWA.

## v3 yenilikleri

- **Kronometre & Odak:** serbest kronometre, 25/50/90 dk ve özel süreli odak zamanlayıcı, tur kayıtları, oturum adı/notu, bugün toplam çalışma süresi, tam ekran.
- **Odak Modu:** arayüzü sadeleştirir. HTTPS üzerinde ve destekleyen tarayıcılarda Screen Wake Lock API ile ekranın uykuya geçmesini önlemeyi dener. Tarayıcı veya cihaz desteklemiyorsa uygulama bunu bildirir.
- **Yanlışlar / Soru Kumbarası:** `accept="image/*"` dosya seçici ile tabletten galeriden birden fazla soru fotoğrafı seçilebilir. Fotoğraflar IndexedDB içinde cihazda tutulur; ders, konu, not ve çözüldü durumu eklenebilir.
- **Denemeler:** TYT için Türkçe 40, Sosyal 20, Matematik 40, Fen 20; AYT için Matematik 40, Fizik 14, Kimya 13, Biyoloji 13. Her dersin doğru/yanlış alanı ayrı, boş ve net otomatik hesaplanır.
- Eski deneme kayıtları korunur; yeni ders dağılımı yeni formatta girilebilir.
- Service Worker önbelleği v3 olarak güncellendi.

## GitHub Pages

ZIP'i açtıktan sonra içindeki dosyaları repository'nin **ana dizinine** koy:

```text
index.html
manifest.json
sw.js
icon-192.png
icon-512.png
README.md
```

Ardından GitHub'da **Settings → Pages → Deploy from a branch → main → /(root)** seç.

## Önemli notlar

Web uygulamaları Android/iPadOS galerisine native uygulama gibi kalıcı bir “tüm galeri izni” alamaz. `input type="file" accept="image/*"` kullanıcı dokunduğunda işletim sisteminin dosya/fotoğraf seçicisini açar; gerekiyorsa izin penceresini işletim sistemi/tarayıcı gösterir. Seçilen fotoğraflar uygulamanın yerel IndexedDB arşivine kopyalanır.

Screen Wake Lock yalnızca HTTPS gibi güvenli bağlamlarda ve destekleyen tarayıcılarda çalışır; cihazın pil/enerji politikası yine kilidi serbest bırakabilir.

Fotoğraf arşivi JSON yedeğine dahil değildir. Fotoğraflar cihazdaki tarayıcı depolamasında tutulur.
