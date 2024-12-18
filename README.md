## Human Activity Recongnition

Bu depo,  sensör verilerine dayalı insan hareketi sınıflandırması yapmak amacıyla geliştirilmiş bir makine öğrenmesi projesinin içeriğini barındırmaktadır. Amaç, ivmeölçer ve jiroskop sensör verilerini kullanarak oturma, koşma, zıplama, eğilme ve forehand gibi insan aktivitelerini tanımaktır.

## Veri Seti

Veri seti, sensör verilerini içermektedir:
- **Jiroskop verileri**: 3 eksenli veri (`gyro_x`, `gyro_y`, `gyro_z`)
- **İvmeölçer verileri**: 3 eksenli veri (`acc_x`, `acc_y`, `acc_z`)

## Modeller

Bu projede insan hareketlerini sınıflandırmak için birden fazla makine öğrenmesi modeli uygulanmıştır:

1. **K-En Yakın Komşu (KNN)**
2. **Karar Ağaçları (Decision Tree)**
3. **Naive Bayes**
4. **Rastgele Orman (Random Forest)**
5. **Destek Vektör Makinesi (SVM)**

Her bir model,  sensör verilerinden çıkartılan özelliklerle eğitilmiş ve doğrulama sonuçları, test verileri kullanılarak değerlendirilmiştir. Bu modellerin performansı doğruluk, precision (doğruluk), recall (duyarlılık) ve F1-skore gibi metriklerle ölçülmüştür.

## Sonuçlar
| Model           | Test Doğruluğu | Eğitim Doğruluğu | Precision     | Recall        | F1-Skoru      |
|-----------------|----------------|------------------|---------------|---------------|---------------|
| KNN             | 0.99987        | 0.99997          | 0.99987       | 0.99987       | 0.99987       |
| Rastgele Orman  | 0.99987        | 1.00000          | 0.99987       | 0.99987       | 0.99987       |
| SVM             | 0.99529        | 0.99623          | 0.99531       | 0.99529       | 0.99529       |
| Karar Ağacı     | 0.99341        | 1.00000          | 0.99341       | 0.99341       | 0.99341       |
| Naive Bayes     | 0.92695        | 0.92415          | 0.92967       | 0.92695       | 0.92636       |
