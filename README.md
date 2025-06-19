# 📚 Akıllı Ders Başarı Tahmin Sistemi / Smart Course Success Prediction System

---

## 📌 Proje Hakkında / About the Project

**Türkçe:**  
Bu proje, öğrencilerin ders başarı durumlarını (geçme/kalma) geçmiş performans, devamsızlık ve sosyal özellikler gibi faktörlere dayanarak tahmin etmeyi amaçlar. Model olarak Random Forest sınıflandırıcısı kullanılmıştır. Veri seti UCI Machine Learning Repository’den alınan “Student Performance Dataset” (Matematik dersi) kullanılmıştır.

**English:**  
This project aims to predict students' course success (pass/fail) based on factors such as past performance, attendance, and social features. A Random Forest classifier is employed for modeling. The dataset is the “Student Performance Dataset” (Math course) from UCI Machine Learning Repository.

---

## 📊 Veri Seti / Dataset Overview

| Özellik (Feature)       | Açıklama (Description)                              |
|------------------------|----------------------------------------------------|
| `school`               | Okul ismi (GP veya MS) / School name (GP or MS)    |
| `sex`                  | Cinsiyet (F/M) / Gender (F/M)                      |
| `age`                  | Yaş (15-22) / Age (15-22)                          |
| `address`              | Yerleşim yeri (urban/rural) / Home address type    |
| `famsize`              | Aile büyüklüğü (LE3 – ≤3 kişi, GT3 – >3 kişi)      |
| `Pstatus`              | Ebeveynlerin birlikte yaşayıp yaşamadığı (T/F)    |
| `Medu`                 | Anne eğitim seviyesi (0-4) / Mother's education     |
| `Fedu`                 | Baba eğitim seviyesi (0-4) / Father's education     |
| `traveltime`           | Okula gidiş süresi (1-4) / Travel time to school   |
| `studytime`            | Haftalık çalışma süresi (1-4) / Weekly study time  |
| `failures`             | Önceki başarısızlık sayısı (0-3) / Past failures   |
| `schoolsup`            | Okul destek programı (yes/no) / School support     |
| `famsup`               | Aile destek programı (yes/no) / Family support     |
| `paid`                 | Ek ücretli ders (yes/no) / Extra paid classes       |
| `activities`           | Okul dışı aktiviteler (yes/no) / Extracurricular activities |
| `higher`               | Yüksek öğrenim isteği (yes/no) / Wants higher education |
| `internet`             | İnternet erişimi (yes/no) / Internet access         |
| `romantic`             | Romantik ilişki durumu (yes/no) / Romantic relationship status |
| `famrel`               | Aile ilişkisi kalitesi (1-5) / Quality of family relationships |
| `freetime`             | Boş zaman kalitesi (1-5) / Free time after school   |
| `goout`                | Sosyal çıkma sıklığı (1-5) / Going out frequency   |
| `Dalc`                 | Haftaiçi alkol tüketimi (1-5) / Workday alcohol consumption |
| `Walc`                 | Haftasonu alkol tüketimi (1-5) / Weekend alcohol consumption |
| `health`               | Sağlık durumu (1-5) / Current health status         |
| `absences`             | Devamsızlık sayısı (0-93) / Number of absences      |
| `G1`                   | 1. sınav notu (0-20) / First period grade           |
| `G2`                   | 2. sınav notu (0-20) / Second period grade          |
| `G3`                   | Final sınav notu (0-20) / Final grade (target)      |

---

## 📈 Temel İstatistikler / Basic Statistics

| Metrik                        | Değer (Value)          | Açıklama (Explanation)                      |
|------------------------------|------------------------|---------------------------------------------|
| Toplam öğrenci sayısı         | 395                    | Total number of students                     |
| Başarılı öğrenci oranı (pass) | %67                    | Percentage of students who passed (G3 ≥ 10) |
| Başarısız öğrenci oranı (fail)| %33                    | Percentage of students who failed (G3 < 10) |
| Ortalama final notu (G3)       | 11.9                   | Average final grade                          |
| Minimum final notu             | 0                      | Minimum grade                               |
| Maksimum final notu            | 20                     | Maximum grade                               |
| Ortalama devamsızlık          | 4.4 gün                | Average number of absences                   |

---

## 🎯 Model Performansı / Model Performance

| Metrik                      | Değer (Value)          | Açıklama (Explanation)                          |
|-----------------------------|------------------------|------------------------------------------------|
| Doğruluk (Accuracy)          | %91                    | Overall accuracy of the model                   |
| Precision (Başarısız sınıfı) | 83%                    | Precision for the fail class                     |
| Recall (Başarısız sınıfı)   | 93%                    | Recall for the fail class                        |
| F1-Score (Başarısız sınıfı) | 88%                    | F1 score for the fail class                      |
| Precision (Başarılı sınıfı)  | 96%                    | Precision for the pass class                     |
| Recall (Başarılı sınıfı)    | 90%                    | Recall for the pass class                         |

---

## 📉 Görselleştirmeler / Visualizations

- Başarı Durumu Dağılımı / Pass-Fail Distribution  
- Modelin Önem Verdiği Özellikler / Top Feature Importances  
- Karmaşıklık Matrisi / Confusion Matrix  

---
