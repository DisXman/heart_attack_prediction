Kalp Hastalığı Tahmini - Makine Öğrenimi Projesi

Bu Python kodu, bir kalp hastalığı tahmini modeli geliştirmek için veri ön işleme, görselleştirme ve sınıflandırma algoritmalarını kullanır. Projenin temel amacı, bir bireyin belirli sağlık verilerine dayanarak kalp hastalığına sahip olup olmadığını tahmin etmektir.

Özellikler
Veri Yükleme ve Keşifsel Veri Analizi (EDA):

Veri Kümesi: Kalp hastalığı verilerini içeren bir CSV dosyası yüklenir.
Keşifsel Veri Analizi: Verinin yapısı, eksik değerler ve sütunların temel istatistiksel özellikleri incelenir.
Hedef Değişken Dönüşümü: Çıkış sütunundaki (output) değerler daha okunabilir olması için haritalanır.
Veri Görselleştirme:

Cinsiyet Dağılımı (Pie Chart): Veri setindeki sex sütunu bir pasta grafiği ile görselleştirilir.
KDE (Kernel Density Estimation) Grafikleri: age, chol, thalachh, ve trtbps sütunları hedef değişkene göre analiz edilir.
Dengesiz Veri İşleme:

SMOTEENN Kullanımı: Dengesiz veri setlerini işlemek için SMOTE (sahte örnekleme) ve ENN (gürültü temizleme) kombinasyonu uygulanır.
Makine Öğrenimi Modelleri:

Modeller: İki model kullanılmıştır:
Random Forest Classifier
Support Vector Machine (SVM)
Veri Ayrımı: Eğitim ve test seti (%80 - %20) oluşturulur.
Standartlaştırma: Eğitim ve test verileri, StandardScaler ile normalize edilir.
Model Eğitimi ve Değerlendirme:

Eğitim seti ile modeller eğitilir.
Test seti üzerinde tahminler yapılır ve modellerin doğruluğu (accuracy) hesaplanır.
Sonuçlar, pandas DataFrame formatında tablo haline getirilir.
