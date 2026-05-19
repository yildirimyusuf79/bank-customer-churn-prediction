# Bank Customer Churn Prediction

Müşteri kaybını (churn) önceden tahmin ederek bankaların riskli müşterileri belirlemesini hedefleyen veri bilimi projesi.
Çalışma, keşifsel veri analizi (EDA), özellik hazırlama ve sınıflandırma modellerinin karşılaştırılması adımlarını notebook tabanlı bir akışla sunar.

## İçerik

- [Proje Özeti](#proje-özeti)
- [İş Problemi](#iş-problemi)
- [Veri Seti](#veri-seti)
- [Proje Yapısı](#proje-yapısı)
- [Yöntem](#yöntem)
- [Kurulum ve Çalıştırma](#kurulum-ve-çalıştırma)
- [Değerlendirme Metrikleri](#değerlendirme-metrikleri)
- [Geliştirme Yol Haritası](#geliştirme-yol-haritası)
- [Katkı](#katkı)
- [Lisans](#lisans)
- [İletişim & Bağlantılar](#iletişim--bağlantılar)

## Proje Özeti

Bu repository, banka müşteri davranışlarını kullanarak churn tahmini yapmayı amaçlar.
Amaç sadece model kurmak değil, aynı zamanda churn kararını etkileyen değişkenleri analiz ederek iş tarafına uygulanabilir içgörüler sunmaktır.

## İş Problemi

Müşteri kaybı, finans sektöründe gelir ve sadakat açısından kritik bir risktir.
Bu projede şu sorulara yanıt aranır:

- Hangi müşteri profilleri churn etme eğilimindedir?
- Churn olasılığını en iyi tahmin eden model hangisidir?
- Metrik bazlı olarak operasyonel kararlar nasıl desteklenebilir?

## Veri Seti

- Dosya: `Churn_Modelling.csv`
- Hedef değişken: `Exited` (0 = müşteri kaldı, 1 = müşteri ayrıldı)
- Veri alanı: demografik bilgiler, finansal durum, hesap davranışları, ürün kullanım göstergeleri

## Proje Yapısı

- `eda.ipynb`: Veri keşfi, dağılımlar, korelasyon incelemeleri, temel bulgular
- `modeller.ipynb`: Model eğitimi, karşılaştırma ve metrik bazlı performans analizi
- `proje.ipynb`: Uçtan uca deney akışı ve sonuçların bir arada sunumu
- `Churn_Modelling.csv`: Ham veri kaynağı

## Yöntem

1. Veri kalite kontrolü ve ilk inceleme
2. Gerekli ön işleme adımları (kodlama, ölçeklendirme, özellik hazırlama)
3. Sınıflandırma modellerinin eğitimi
4. Performans karşılaştırması ve yorumlama
5. İş etkisi açısından bulguların değerlendirilmesi

## Kurulum ve Çalıştırma

### 1. Projeyi klonlayın

```bash
git clone https://github.com/yildirimyusuf79/bank-customer-churn-prediction.git
cd bank-customer-churn-prediction
```

### 2. Sanal ortam oluşturun

```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate
```

### 3. Bağımlılıkları yükleyin

```bash
pip install jupyter pandas numpy matplotlib seaborn scikit-learn
```

### 4. Notebookları çalıştırın

```bash
jupyter notebook
```

Çalışma sırası önerisi:

1. `eda.ipynb`
2. `modeller.ipynb`
3. `proje.ipynb`

## Değerlendirme Metrikleri

Model performansı aşağıdaki metriklerle değerlendirilir:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC

Not: Churn problemi iş hedefine göre Precision-Recall dengesi ile yorumlanmalıdır.

## Geliştirme Yol Haritası

- Hiperparametre optimizasyonu (GridSearchCV / RandomizedSearchCV)
- Sınıf dengesizliği yöntemleri (class weight, SMOTE)
- Model açıklanabilirliği (SHAP, LIME)
- Notebook akışının modüler Python yapısına taşınması
- Basit bir API veya dashboard ile modelin sunuma hazır hale getirilmesi

## Katkı

Katkı sağlamak için issue açabilir veya pull request gönderebilirsiniz.

## Lisans

Bu proje eğitim ve portfolyo amaçlı paylaşılmıştır.
Üretim ortamı kullanımları için ek doğrulama, test ve izleme katmanları önerilir.

## 📞 İletişim & Bağlantılar

- Repository: [github.com/yildirimyusuf79/malatya-su-talebi-projesi](https://github.com/yildirimyusuf79/malatya-su-talebi-projesi)
- LinkedIn: [www.linkedin.com/in/yusuf-yıldırım-190445295](https://www.linkedin.com/in/yusuf-y%C4%B1ld%C4%B1r%C4%B1m-190445295)
- Geliştirici: Yusuf Yıldırım
