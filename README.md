# 📉 Customer Churn Prediction (Müşteri Terk Tahmini)

Bu proje, makine öğrenmesi algoritmaları kullanılarak müşterilerin bir hizmeti bırakıp bırakmayacağını (churn) tahmin eden bir sınıflandırma modelidir.

## 🚀 Proje Hakkında
Müşteri kaybı (Churn), işletmeler için kritik bir metriktir. Bu çalışmada, müşterilerin demografik bilgileri ve hesap hareketleri analiz edilerek potansiyel kayıpların önceden tespit edilmesi amaçlanmıştır.

**Temel Hedef:** Verilen özniteliklere (feature) dayanarak müşterinin "Terk Eden" (1) veya "Kalan" (0) olduğunu yüksek doğrulukla tahmin etmek.

## 📂 Veri Seti (Dataset)
Bu projede kullanılan veri seti Kaggle'dan alınmıştır. Dosya boyutu ve lisans standartları gereği veri seti repoya dahil edilmemiştir.

👉 **Veri Setine buradan ulaşabilirsiniz:** [https://www.kaggle.com/datasets/blastchar/telco-customer-churn]

* **Veri Kaynağı:** Kaggle
* **Hedef Değişken:** `Exited` (Churn)

## 🛠️ Kullanılan Teknolojiler
* **Dil:** Python
* **Kütüphaneler:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, SHAP
* **Ortam:** Jupyter Notebook

## 📊 Model Başarısı
Modelin test verisi üzerindeki performans metrikleri aşağıdadır:

| Sınıf | Precision | Recall (Duyarlılık) | F1-Score | Destek (Kişi) |
| :--- | :--- | :--- | :--- | :--- |
| **0 (Kalacak Müşteri)** | 0.93 | 0.67 | 0.78 | 1036 |
| **1 (Gidecek Müşteri)** | **0.49** | **0.86** 🚀 | 0.62 | 373 |

> **Not:** Kodun temiz ve incelenebilir olması için `.ipynb` dosyası çıktısız (outputsuz) yüklenmiştir. Tüm sonuç grafikleri aşağıda mevcuttur.

## 📈 Analiz ve Görselleştirmeler

### 1. Confusion Matrix (Karmaşıklık Matrisi)
Modelin doğru ve yanlış tahminlerinin dağılımı:

![Confusion Matrix](outputs/Confusion%20Matrix.png)

### 2. Feature Importance (Öznitelik Önemi)
Müşteri terk kararını en çok etkileyen faktörlerin sıralaması:

![Feature Importance](outputs/Feature%20Importance.png)

### 3. SHAP Değerleri (Model Açıklanabilirliği)
Modelin kararlarını nasıl verdiğini gösteren SHAP analizi:

![SHAP Analizi](outputs/Shap.png)

## ⚙️ Kurulum

Projeyi kendi bilgisayarınızda çalıştırmak için:

1. Repoyu klonlayın:
   ```bash
   git clone [https://github.com/EmirhanKisa/customer-churn-prediction.git](https://github.com/EmirhanKisa/customer-churn-prediction.git)
