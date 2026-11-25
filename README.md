# Mikro Fark 2.0

Yerel çalışan, tek HTML tabanlı karşılaştırma laboratuvarı. GitHub Pages'e yayınlanabilir.

## 2.0 ekleri
- CSV anahtar kolonuna göre kayıt eşleştirme: değişen, eklenen, silinen kayıtları key üzerinden tespit eder; tekrar eden key'leri hata olarak bildirir.
- Binary/Hex compare: dosyaları byte bazında inceler, hex/ASCII satırlarını gösterir, farklı satırları filtreleyebilir.
- 8 MB dosya sınırı (Hex gösterimi); daha büyük dosyalar için kullanmayın.
- İlk sürümdeki metin, kod, JSON, CSV sıra bazlı, görsel, hash, dosya listesi, rapor, tema ve isteğe bağlı geçmiş özellikleri.

## Yayın
`index.html` dosyasını GitHub repository ana dizinine yükleyin. Settings → Pages → Deploy from a branch → main → root.

## Gizlilik ve sınırlar
Dosyalar tarayıcı içinde okunur; uygulama kaynak kodunda dış servis veya API çağrısı yoktur. Hash için Web Crypto API gerekir. Hex karşılaştırma dosya başına 8 MB ile sınırlandırılmıştır. CSV key matching seçilen kolonlar üzerinden yapılır; duplicate keys hata verir. Bu paket Worker tabanlı diff, ZIP açma, gerçek offline PWA cache ve Android testleri içermez; tamamlanmış gibi sunulmamaktadır.
