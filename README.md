# YKS 2027 • Akıllı Koç PWA

Bu paket, GitHub Pages üzerinden yayınlanabilen tek sayfalı bir PWA'dır.

## İçerik
- Ana sayfa: YKS 2027 geri sayım, günlük özet, tekrar kuyruğu, son denemeler
- Konular: TYT/AYT ders-konuları, durum + ustalık + soru/doğru + tekrar tarihi
- Akıllı Planlayıcı: günlük görev, aylık görünüm ve otomatik öneriler
- Denemeler: doğru/yanlış/boş otomatik hesaplama, düzenleme, hata konusu seçimi
- Bilimsel Tekrar: 1/3/7/14/30/60 gün basamaklı tekrar
- Kronometre: sayfa değişiminde korunan süre, tur işaretleri ve tam ekran
- Hedefler: net hedefleri, üniversite/bölüm hedefi
- Raporlar: net trendi, konu tamamlanma, öncelikli konular, aylık özet
- Yanlışlar: deneme hatalarını toplu görme ve plana ekleme
- Ayarlar: tema, sınav tarihi, JSON yedekleme/geri yükleme

## GitHub Pages
1. ZIP'i çıkar.
2. ZIP açıldığında görünen `index.html`, `manifest.json`, `sw.js` ve ikon dosyalarını **doğrudan repository ana dizinine** yükle. `YKS_2027_Akilli_Koc` adlı ek bir klasör oluşturup onun içine koyma.
3. Settings → Pages → Deploy from branch → `main` / root seç.
4. HTTPS adresinden tabletten aç.
5. Tarayıcı destekliyorsa “Uygulamayı yükle” seçeneği ile ana ekrana ekle.

## Veri
Kişisel ilerleme verileri `localStorage` içinde cihaz/tarayıcıda tutulur. GitHub Pages'e kişisel çalışma verisi gönderilmez.

## 2027 tarihi notu
Varsayılan hedef tarih 19 Haziran 2027'dir ve uygulama bunu tahmini olarak işaretler. 2027 YKS'nin resmi tarihi ÖSYM tarafından yayımlandığında Ayarlar bölümünden tek dokunuşla güncellenmelidir.
