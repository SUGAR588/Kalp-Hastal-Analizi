# Kalp Hastalığı Risk Tahmini (Heart Disease Prediction)

Bu proje, makine öğrenmesi algoritmaları kullanılarak bireylerin klinik verilerine dayanarak kalp hastalığı riskini tahmin etmeyi amaçlamaktadır. Veri Analizi dersi kapsamında geliştirilmiştir.

## 🎯 Projenin Amacı
Kalp hastalıkları dünya genelinde önde gelen ölüm nedenlerinden biridir. Bu projenin amacı, yaş, kolesterol, kan basıncı gibi temel sağlık verilerini analiz ederek, bir kişinin kalp hastası olup olmadığını (Sınıflandırma Problemi) yüksek doğrulukla tahmin eden bir model geliştirmektir.

## 📊 Veri Seti
Kullanılan veri seti Kaggle platformundan temin edilmiştir: **Heart Disease UCI**
* **Veri Sayısı:** 270 Gözlem
* **Öznitelik Sayısı:** 13 Bağımsız Değişken (Yaş, Cinsiyet, Göğüs Ağrısı Tipi, vb.) + 1 Hedef Değişken

## 🚀 Kullanılan Teknolojiler
* **Dil:** Python
* **Kütüphaneler:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
* **Ortam:** Jupyter Notebook

## ⚙️ Uygulanan Adımlar
1. **Veri Keşfi (EDA):** Veri setindeki dengesizlikler ve korelasyonlar incelendi.
   - *Bulgu:* Göğüs ağrısı (Chest Pain) ve Maksimum Kalp Atış Hızı (Max HR) hastalıkla pozitif ilişkili bulundu.
2. **Ön İşleme:**
   - Kategorik veriler (Presence/Absence) sayısal değerlere (1/0) dönüştürüldü.
   - Veriler `StandardScaler` ile ölçeklendirilerek modellerin performansı artırıldı.
3. **Modelleme:** İki farklı algoritma karşılaştırmalı olarak eğitildi:
   - Lojistik Regresyon (Logistic Regression)
   - Rastgele Orman (Random Forest Classifier)

## 📈 Sonuçlar

Test verisi üzerinde yapılan değerlendirmeler sonucunda elde edilen başarı oranları şöyledir:

| Model | Doğruluk Oranı (Accuracy) |
|-------|---------------------------|
| **Lojistik Regresyon** | **%90.74** |
| Random Forest | %75.93 |

### Değerlendirme
Beklenenin aksine, daha basit bir yapıya sahip olan **Lojistik Regresyon** modeli, Random Forest modeline göre belirgin bir üstünlük sağlamıştır
