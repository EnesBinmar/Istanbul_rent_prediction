# 🏠 İstanbul Kiralık Konut Fiyat Tahmin Modeli

Bu proje, İstanbul'daki kiralık konut ilanlarından elde edilen verilerle, konut fiyatlarını tahmin etmek amacıyla geliştirilmiştir. Model, çeşitli makine öğrenimi algoritmaları ile test edilerek en iyi performansı veren yapı optimize edilmiştir.

## 🔍 Proje Amacı

- İstanbul'daki kiralık ev fiyatlarını etkileyen faktörleri analiz etmek
- Uygun özelliklerle beslenen bir makine öğrenimi modeli oluşturmak
- Kullanıcıların ev kiralama sürecinde fiyatın makul olup olmadığını istatistiksel olarak değerlendirebilmesini sağlamak

## 📊 Kullanılan Veri Seti

Veri seti, İstanbul genelindeki kiralık konut ilanlarından toplanmıştır. Toplam **6000+** ilan verisi içermektedir. Veride yer alan başlıca özellikler:

- İlçe ve mahalle bilgisi
- Metrekare
- Oda sayısı
- Bina yaşı
- Kat bilgisi
- Fiyat

## 🧠 Kullanılan Yöntemler

- **Veri Ön İşleme** (Eksik verilerin giderilmesi, aykırı değerlerin temizlenmesi)
- **Feature Engineering** (Yeni özellikler üretme ve kategorik verilerin encode edilmesi)
- **Modelleme**:  
  - Linear Regression  
  - Random Forest Regressor  
  - Gradient Boosting  
  - XGBoost

- **Model Seçimi**:  
  - GridSearchCV ile hiperparametre optimizasyonu  
  - Cross-Validation ile model doğrulama

## 📈 Model Performansı

Model performansları eğitim ve test seti üzerinde R² (determinasyon katsayısı) ve MSE (ortalama kare hatası) metrikleriyle değerlendirilmiştir.

| Veri Seti | MSE   | R²     |
|-----------|-------|--------|
| Eğitim    | 0.30  | 0.91   |
| Test      | 0.53  | 0.72   |

## 🚀 Gelecek Planlar

Projeyi bir mobil uygulamaya entegre ederek kullanıcıların kiralamak istedikleri evin özelliklerini girip sistemden istatistiksel fiyat tahmini alabilecekleri bir platforma dönüştürmek hedeflenmektedir.

## 📎 Bağlantılar

- 📁 [Proje Dosyaları](https://github.com/EnesBinmar/Istanbul_rent_prediction.git)
- 📬 Bana ulaşmak için: [LinkedIn Profilim](https://www.linkedin.com/in/___senin-profilin___)

## ⚙️ Gereksinimler

Projenin çalışması için gereken temel kütüphaneler:
```bash
pandas
numpy
scikit-learn
xgboost
matplotlib
seaborn
