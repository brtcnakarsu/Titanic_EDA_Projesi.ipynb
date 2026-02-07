# Titanic_EDA_Projesi.ipynb
Titanic - Machine Learning from Disaster

# 🚢 Titanic - Exploratory Data Analysis (EDA)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Library](https://img.shields.io/badge/Library-Pandas%20%7C%20Seaborn-orange)
![License](https://img.shields.io/badge/License-MIT-green)

## 📌 Proje Hakkında
Bu proje, veri biliminin "Hello World"ü olarak kabul edilen meşhur **Titanic Veri Seti** üzerinde gerçekleştirilmiş bir Keşifçi Veri Analizi (Exploratory Data Analysis) çalışmasıdır.

Analizin temel amacı; yolcuların demografik özelliklerini incelemek, hayatta kalma oranlarını etkileyen faktörleri (sınıf, cinsiyet, yaş vb.) görselleştirmek ve veri setindeki eksik bilgileri istatistiksel yaklaşımlarla temizlemektir.

## 📊 Kullanılan Teknolojiler
Bu projede aşağıdaki Python kütüphaneleri kullanılmıştır:
* **Pandas:** Veri manipülasyonu ve analizi için.
* **NumPy:** Sayısal işlemler için.
* **Matplotlib & Seaborn:** Veri görselleştirme (Heatmap, Countplot, Boxplot) için.

## ⚙️ Yapılan İşlemler (Methodology)

### 1. Veri İnceleme
* Veri setinin genel yapısı, değişken tipleri ve istatistiksel özetleri (`describe`, `info`) incelendi.

### 2. Eksik Veri Analizi (Missing Value Analysis)
* Veri setindeki eksik değerler `Heatmap` kullanılarak görselleştirildi.
* `Cabin` sütunu çok fazla eksik veri içerdiği için veri setinden çıkarıldı.
* **Kritik Adım:** `Age` (Yaş) sütunundaki eksik veriler, veri setinin genel ortalaması yerine, yolcuların **Bilet Sınıfına (Pclass) göre yaş ortalamaları** baz alınarak dolduruldu.

> **Not:** Yaş ataması yapılırken "Mean Imputation" yöntemi kullanılmıştır. Bu yöntem varyansı düşürebileceği için, ilerleyen aşamalarda standart sapma bazlı rastgele atama yöntemleri de değerlendirilebilir.

### 3. Veri Görselleştirme & Bulgular
Veri seti görselleştirildiğinde aşağıdaki içgörülere ulaşılmıştır:
* **Cinsiyet:** Kadınların hayatta kalma oranı erkeklere göre belirgin şekilde yüksektir.
* **Sınıf Farkı:** 1. Sınıf yolcuların hayatta kalma oranı, 3. Sınıf yolculara göre daha fazladır.
* **Yaş Dağılımı:** Yolcu kitlesi ağırlıklı olarak genç yetişkinlerden (20-35 yaş) oluşmaktadır.

---

## 📈 Örnek Grafikler

<img width="571" height="455" alt="indir (1)" src="https://github.com/user-attachments/assets/f4d4b905-dcc0-4876-a94e-b8eb5aad2833" />
<img width="695" height="470" alt="indir" src="https://github.com/user-attachments/assets/04db6576-c77e-4e25-9fc1-a34066ae594b" />


---

## 🚀 Nasıl Çalıştırılır?
1. Repoyu klonlayın:
   ```bash
   git clone [https://github.com/KULLANICI_ADIN/Titanic-EDA-Analysis.git](https://github.com/KULLANICI_ADIN/Titanic-EDA-Analysis.git)
