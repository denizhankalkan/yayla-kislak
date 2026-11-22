# Yayla & Kışlak

Niğde (Çukurbağ, Çamardı), Çukurova, Hatay ve Antep'teki kooperatiflerden ve küçük üreticilerden organik ürünler satan e-ticaret sitesinin ön yüzü.

- Tek sayfa, bağımlılıksız HTML/CSS/JS (`index.html`)
- Türkçe / İngilizce dil desteği
- Ürün listesi, kategori filtresi, sıralama, sepet (tarayıcıda saklanır)
- **Yayla & Kışlak modeli**: hasattan önce ödeme, aracısız, toplu gönderim; elma örneğiyle rakamlar ve hasat takvimi
- **Ağaç Sahiplen**: elma, kiraz, ceviz; tam / yarım / çeyrek pay; 1 ya da 3 yıl; ağaca isim (levha önizlemesi), hediye, SSS, kurumsal bölüm
- **Tarla Payı**: Niğde patatesi ve kuru soğanı için ekimden önce ön sipariş; İstanbul teslim günü ya da kargo
- **Şeffaf fiyat**: her fiyat üretici fiyatından hesaplanır ve "Paranız nereye gidiyor?" tablosunda gösterilir

## Fiyat hesabı

`index.html` içindeki `TREES`, `FIELD`, `DELIV` ve `FIX/COMM/OURS` sabitleri fiyatları belirler:

- Ağaç: (kg × (üretici fiyatı + kargo + ambalaj) + levha/sertifika) ÷ (1 − %3 komisyon − %18 Yayla & Kışlak payı), 50 ₺'ye yuvarlanır. 3 yılda %10 indirim, üretici payı değişmez.
- Tarla Payı: aynı hesap, Yayla & Kışlak payı %12.
- Elma: ağaç başına 100 kg (4 × 25 kg kasa), üreticiye 30 ₺/kg (tüccar 10 ₺ veriyordu), İstanbul 80–150 ₺/kg. Kiraz, ceviz, patates ve soğan rakamları örnektir.
- Fotoğraflar `img/` klasöründe

## Çalıştırma

`index.html` dosyasını tarayıcıda açmak yeterli. Yayına almak için GitHub Pages, Netlify ya da Render kullanılabilir.

## Yapılacaklar

- Gerçek ürün fotoğrafları, fiyatlar ve üretici bilgileri
- Ödeme altyapısı (iyzico / PayTR)
- Üyelik ve sipariş yönetimi
- Bülten servisi
- Kiraz, ceviz, patates, soğan için gerçek verim ve üretici fiyatları
- Gerçek kiraz, ceviz, patates ve soğan fotoğrafları
- Numaralı ağaç listesi ve paylaşılan ağaçlarda doluluk takibi, sertifika şablonu
- Anlaşmalı kargo ve İstanbul teslim noktaları
