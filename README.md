# sirket-veri-raporu
CSV dosyasından çalışan verisi okuyup analiz raporu üreten Python scripti.
# Şirket Çalışan Veri Raporu

CSV formatındaki çalışan verisini okuyup analiz eden ve formatlı bir rapor 
dosyası üreten Python scripti.

## Ne yapar?

- Şirket çalışanlarının verisini CSV dosyasından okur
- Sayısal sütunları uygun tipe çevirir (tam sayı / ondalık)
- Toplam ve ortalama metrikleri hesaplar (maaş, yaş, performans, çalışma yılı)
- En yüksek ve en düşük maaş ile performansı bulan çalışanları belirler
- Departman bazında çalışan sayımı yapar
- Belirli bir şehirdeki çalışanları filtreler
- Sonuçları formatlı bir rapor dosyası olarak yazar

## Kullanılan kavramlar

- Dosya okuma/yazma (`open`, `read`, `write`)
- Sözlük ve liste veri yapıları
- Döngüler ve koşullu mantık
- String işleme (`strip`, `split`)
- f-string ile formatlı çıktı

## Nasıl çalıştırılır?

1. `sirket.csv` ve `sirketraporu.ipynb` aynı klasörde olmalı
2. Jupyter Notebook ile `sirketraporu.ipynb` aç
3. Hücreleri sırayla çalıştır
4. Çıktı olarak `rapor2.txt` dosyası oluşur

## Dosyalar

- `calisan_raporu.ipynb` — Ana Python kodu
- `sirket.csv` — Örnek çalışan verisi (12 kayıt)
- `rapor2.txt` — Üretilen rapor (örnek çıktı)
