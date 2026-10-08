# YKS 2027 • Akıllı Koç v5.1 PRO

Tablet ve GitHub Pages için hazırlanmış PWA.

## v5.1 PRO değişiklikleri
- Akıllı Planlayıcı / Koçun Anlık Önerileri: güvenli indeks tabanlı "Plana Ekle" akışı.
- Sayısal Aktif Koç: günlük saat hedefi + hafif/orta/zor mod + aktif sohbet + TYT→AYT kademeli yol haritası.
- Koçun konu önerileri yalnızca TYT Matematik, TYT Fizik, TYT Kimya, TYT Biyoloji, TYT Geometri ve hazır oldukça bunların AYT karşılıklarından üretilir.
- Her gün paragraf + problem + geometri rutini; 2–3 günde bir TYT Sosyal özet okuması ayrı rutin olarak planlanır.
- PRO Raporlar: aylık seçim, çalışma hacmi, görev disiplini, konu ilerleyişi, deneme trendi, sayısal ders tablosu ve gelecek hafta/ay tavsiyeleri.
- Aylık rapor için PDF'e kaydetmeye uygun A4 yazdırma görünümü.
- Service Worker cache sürümü 5.1.1.

## GitHub Pages
Dosyaları repository kök dizinine koy:

- index.html
- manifest.json
- sw.js
- icon-192.png
- icon-512.png
- README.md

Settings → Pages → Deploy from a branch → main → /(root)

## Aylık PDF
Raporlar > Aylık PDF raporu düğmesi tarayıcının yazdırma ekranını açar. Buradan "PDF olarak kaydet" seçilebilir. Bu yöntem harici PDF kütüphanesi gerektirmeden çevrimdışı PWA ile çalışır.


Düzeltme: Akıllı Planlayıcı, Koç ve Raporlar sekmelerindeki eksik global değişkenler giderildi. 11 ana sekme Node tabanlı DOM stub testiyle açılış render testinden geçirildi.
