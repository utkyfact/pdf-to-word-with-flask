# PDF to Word Converter with Flask 🔄

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-2.0%2B-lightgrey)](https://flask.palletsprojects.com/)
[![License](https://img.shields.io/badge/License-MIT-green)](https://opensource.org/licenses/MIT)

Flask tabanlı, OCR destekli PDF'den Word belgesine dönüştürücü uygulaması. Hem metin tabanlı hem de görüntülü PDF'leri destekler.

**Demo:** [Canlı Demo](https://your-domain.com) | **Geliştirici:** [@utkyfact](https://github.com/utkyfact)

## 🌟 Özellikler

- **Çift Modlu Çalışma**
  - Metin tabanlı PDF'ler için direkt dönüşüm
  - Görüntülü/Scan PDF'ler için Tesseract OCR entegrasyonu
- **Çoklu Dil Desteği** (Türkçe & İngilizce)
- **Otomatik Temizlik** (Geçici dosyaları siler)
- Responsive Arayüz
- 16MB Dosya Boyut Limiti

## 🚀 Hızlı Kurulum

### Ön Gereksinimler
- Python 3.10+
- Tesseract OCR ([İndirme Linki](https://github.com/UB-Mannheim/tesseract/wiki))

### Adımlar
1. Depoyu klonlayın:
```bash
git clone https://github.com/utkyfact/pdf-to-word-with-flask.git
cd pdf-to-word-with-flask
