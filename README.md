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

### Saf Python versiyonu
- `sirketraporu.ipynb` — Saf Python ile yazılmış kod
- `rapor2.txt` — Üretilen rapor

### Pandas versiyonu
- `sirket_raporu_pandas.ipynb` — Pandas ile yazılmış kod (daha kısa, daha güçlü)
- `rapor_pandas.txt` — Üretilen rapor (groupby + agg analizleri dahil)

### Ortak
- `sirket.csv` — Örnek çalışan verisi (12 kayıt)

## Notlar

Bu projede aynı analiz iki farklı yaklaşımla yazıldı:
- **Saf Python**: Standart kütüphaneler, döngüler, sözlükler kullanılarak (~80 satır)
- **Pandas**: `pd.read_csv`, `groupby`, `agg` gibi pandas araçlarıyla (~20 satır)

İkinci versiyon hem daha kısa, hem de departman/şehir bazında çapraz analizler içeriyor.
