# Bank Customer Churn Prediction

Bu proje, banka müşterilerinin churn (müşteri kaybı) olasılığını veri analizi ve makine ogrenmesi yaklasimi ile incelemek icin hazirlanmistir. Proje, kesifsel veri analizi (EDA), modelleme denemeleri ve notebook tabanli deneylerden olusur.

## Proje Amaci

- Musteri kaybini etkileyen temel degiskenleri analiz etmek
- Churn tahmini icin siniflandirma modelleri gelistirmek
- Model performansini metrikler uzerinden degerlendirmek
- Is birimleri icin aksiyona donusebilir icgoruler elde etmek

## Veri Seti

- Dosya: `Churn_Modelling.csv`
- Hedef degisken: `Exited` (0 = kaldı, 1 = churn)
- Veri seti; demografik bilgiler, hesap ozellikleri ve urun kullanim bilgileri gibi musteriyi tanimlayan alanlar icerir.

## Proje Yapisi

- `eda.ipynb`: Veri kesfi, dagilimlar, iliskiler ve on analizler
- `modeller.ipynb`: Model kurulumlari, egitim ve performans degerlendirmeleri
- `proje.ipynb`: Uctan uca proje akisi ve deney notlari
- `Churn_Modelling.csv`: Ham veri

## Kullanilan Yaklasim

1. Veri on inceleme ve kalite kontrol
2. Eksik/aykiri deger kontrolu
3. Ozellik muhendisligi ve uygun kodlama/olceklendirme adimlari
4. Siniflandirma modellerinin egitimi
5. Performans metrikleri ile karsilastirma (ornek: Accuracy, Precision, Recall, F1, ROC-AUC)

## Kurulum ve Calistirma

### 1) Depoyu klonlayin

```bash
git clone https://github.com/yildirimyusuf79/bank-customer-churn-prediction.git
cd bank-customer-churn-prediction
```

### 2) Sanal ortam olusturun (onerilir)

```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS / Linux
source .venv/bin/activate
```

### 3) Gerekli paketleri yukleyin

Not: Proje notebook tabanli oldugu icin paketler kullanilan hucrelere gore degisebilir. Tipik paketler:

```bash
pip install jupyter pandas numpy matplotlib seaborn scikit-learn
```

### 4) Notebooklari calistirin

```bash
jupyter notebook
```

Ardindan sirasiyla `eda.ipynb`, `modeller.ipynb` ve `proje.ipynb` dosyalarini acip hucreleri calistirin.

## Beklenen Ciktilar

- Churn davranisini aciklayan temel degiskenlerin belirlenmesi
- Birden fazla modelin performans karsilastirmasi
- Is hedeflerine uygun, yorumlanabilir churn tahmin yaklasimi

## Gelistirme Onerileri

- Hiperparametre optimizasyonu (GridSearchCV, RandomizedSearchCV)
- Sinif dengesizligi icin SMOTE veya class-weight stratejileri
- Model aciklanabilirligi icin SHAP/LIME entegrasyonu
- Notebook akisini Python modullerine tasiyarak uretim hazir hale getirme

## Katki

Katki onerileri, issue ve pull request acabilirsiniz.

## Lisans

Bu proje egitim ve portfolyo amacli kullanima uygundur. Uretim ortami kullanimi oncesinde ek dogrulama tavsiye edilir.
