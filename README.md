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
```
2. Sanal ortam oluşturup bağımlılıkları yükleyin:
```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```
3. Tesseract yolunu ayarlayın (app.py içinde):
```bash
pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'  # Windows
# veya
# pytesseract.pytesseract.tesseract_cmd = '/usr/bin/tesseract'  # Linux/Mac
```
4. Uygulamayı başlatın:
```bash
flask run
```
## 🖥️ Kullanım
1. Tarayıcınızda http://localhost:5000 açın

2. PDF dosyanızı seçin

3. "Dönüştür" butonuna tıklayın

4. Word dosyası otomatik indirilecektir


## 🛠️ Geliştirme
### Yapılandırma
.env dosyası ile ayarları özelleştirin:
```bash
FLASK_DEBUG=0
UPLOAD_FOLDER=uploads
MAX_FILE_SIZE=16777216  # 16MB
```
### Test
```bash
python -m pytest tests/
```
## 🤝 Katkıda Bulunma
1. Forklayın (https://github.com/utkyfact/pdf-to-word-with-flask/fork)

2. Yeni branch oluşturun (git checkout -b feature/fooBar)

3. Değişikliklerinizi commit edin (git commit -am 'Add some fooBar')

4. Push yapın (git push origin feature/fooBar)

5. Pull Request oluşturun

## 📜 Lisans
### MIT Lisansı - Detaylar için LICENSE dosyasına bakın.
Not: Üretim ortamında kullanmadan önce debug=False yapmayı unutmayın. Sorunlar için Issues kısmını kullanabilirsiniz.
```bash
Bu README dosyasını proje kök dizinine `README.md` olarak kaydedebilirsiniz. Gerektiğinde aşağıdaki gibi özelleştirebilirsiniz:

1. Canlı demo linki eklemek için `your-domain.com` yerine gerçek domain
2. Ekran görüntüsü için `via.placeholder.com` yerine gerçek görsel linki
3. Ek özellikler veya kullanım talimatları ekleyebilirsiniz
```