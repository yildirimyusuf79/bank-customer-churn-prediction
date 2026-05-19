# Bank Customer Churn Prediction

Musteri kaybini (churn) onceden tahmin ederek bankalarin riskli musterileri belirlemesini hedefleyen veri bilimi projesi.
Calisma, kesifsel veri analizi (EDA), ozellik hazirlama ve siniflandirma modellerinin karsilastirilmasi adimlarini notebook tabanli bir akisla sunar.

## Icerik

- [Proje Ozeti](#proje-ozeti)
- [Is Problemi](#is-problemi)
- [Veri Seti](#veri-seti)
- [Proje Yapisi](#proje-yapisi)
- [Yontem](#yontem)
- [Kurulum ve Calistirma](#kurulum-ve-calistirma)
- [Degerlendirme Metrikleri](#degerlendirme-metrikleri)
- [Gelistirme Yol Haritasi](#gelistirme-yol-haritasi)
- [Katki](#katki)
- [Lisans](#lisans)

## Proje Ozeti

Bu repository, banka musteri davranislarini kullanarak churn tahmini yapmayi amaclar.
Amac sadece model kurmak degil, ayni zamanda churn kararini etkileyen degiskenleri analiz ederek is tarafina uygulanabilir icgoruler sunmaktir.

## Is Problemi

Musteri kaybi, finans sektorunde gelir ve sadakat acisindan kritik bir risktir.
Bu projede su sorulara yanit aranir:

- Hangi musteri profilleri churn etme egilimindedir?
- Churn olasiligini en iyi tahmin eden model hangisidir?
- Metrik bazli olarak operasyonel kararlar nasil desteklenebilir?

## Veri Seti

- Dosya: `Churn_Modelling.csv`
- Hedef degisken: `Exited` (0 = musteri kaldi, 1 = musteri ayrildi)
- Veri alani: demografik bilgiler, finansal durum, hesap davranislari, urun kullanim gostergeleri

## Proje Yapisi

- `eda.ipynb`: Veri kesfi, dagilimlar, korelasyon incelemeleri, temel bulgular
- `modeller.ipynb`: Model egitimi, karsilastirma ve metrik bazli performans analizi
- `proje.ipynb`: Uctan uca deney akisi ve sonuclarin bir arada sunumu
- `Churn_Modelling.csv`: Ham veri kaynagi

## Yontem

1. Veri kalite kontrolu ve ilk inceleme
2. Gerekli on isleme adimlari (kodlama, olceklendirme, ozellik hazirlama)
3. Siniflandirma modellerinin egitimi
4. Performans karsilastirmasi ve yorumlama
5. Is etkisi acisindan bulgularin degerlendirilmesi

## Kurulum ve Calistirma

### 1. Projeyi klonlayin

```bash
git clone https://github.com/yildirimyusuf79/bank-customer-churn-prediction.git
cd bank-customer-churn-prediction
```

### 2. Sanal ortam olusturun

```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate
```

### 3. Bagimliliklari yukleyin

```bash
pip install jupyter pandas numpy matplotlib seaborn scikit-learn
```

### 4. Notebooklari calistirin

```bash
jupyter notebook
```

Calisma sirasi onerisi:

1. `eda.ipynb`
2. `modeller.ipynb`
3. `proje.ipynb`

## Degerlendirme Metrikleri

Model performansi asagidaki metriklerle degerlendirilir:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC

Not: Churn problemi is hedefine gore Precision-Recall dengesi ile yorumlanmalidir.

## Gelistirme Yol Haritasi

- Hiperparametre optimizasyonu (GridSearchCV / RandomizedSearchCV)
- Sinif dengesizligi yontemleri (class weight, SMOTE)
- Model aciklanabilirligi (SHAP, LIME)
- Notebook akisinin moduler Python yapisina tasinmasi
- Basit bir API veya dashboard ile modelin sunuma hazir hale getirilmesi

## Katki

Katki saglamak icin issue acabilir veya pull request gonderebilirsiniz.

## Lisans

Bu proje egitim ve portfolyo amacli paylasilmistir.
Uretim ortami kullanimlari icin ek dogrulama, test ve izleme katmanlari onerilir.
