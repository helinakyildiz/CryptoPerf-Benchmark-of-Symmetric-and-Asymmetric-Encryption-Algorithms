# CryptoPerf-Benchmark-of-Symmetric-and-Asymmetric-Encryption-Algorithms
# CryptoBenchmark: Şifreleme Algoritmaları Performans Analizi

Bu proje, modern ve klasik şifreleme algoritmalarının (AES, RSA, Blowfish, ChaCha20 ve 3DES) performanslarını farklı veri boyutları üzerinden karşılaştırmalı olarak analiz eder. Python dili kullanılarak geliştirilen bu araç, algoritmaların işlem sürelerini ve bellek (RAM) kullanımlarını ölçerek görselleştirir.

## 🚀 Özellikler

- **Çoklu Algoritma Desteği:** - Simetrik: AES (CBC), Blowfish (CBC), ChaCha20, 3DES (ECB)
  - Asimetrik: RSA (PKCS1_OAEP)
- **Kapsamlı Ölçüm:** `time.perf_counter` ile yüksek hassasiyetli süre ölçümü ve `psutil` ile anlık bellek tüketimi analizi.
- **Dinamik Veri Testi:** 1MB, 5MB ve 10MB boyutlarında rastgele oluşturulan veriler üzerinde otomatik test süreci.
- **Veri Görselleştirme:** Elde edilen sonuçların `matplotlib` kütüphanesi ile sütun grafiklerine dönüştürülmesi.
- **Veri Analizi:** Tüm sonuçların `pandas` DataFrame yapısı ile tablo halinde sunulması.

## 📊 Örnek Analiz Bulguları

Yapılan testlerde genel olarak şu gözlemler yapılmıştır:
- **ChaCha20**, en düşük gecikme süresiyle en hızlı çalışan algoritma olarak öne çıkmaktadır.
- **RSA**, asimetrik doğası gereği büyük verilerde işlem yükü en yüksek olan algoritmadır.
- **3DES**, güncel rakiplerine (AES, ChaCha20) göre belirgin şekilde daha yavaş performans göstermektedir.

## 🛠 Kurulum ve Çalıştırma

Projenin yerelinizde çalışması için gerekli bağımlılıkları yükleyin:

```bash
pip install cryptography pycryptodome psutil matplotlib tqdm pandas
Ardından, Jupyter Notebook dosyasını (.ipynb) herhangi bir IDE (VS Code, PyCharm vb.) veya Google Colab üzerinde çalıştırabilirsiniz.
