MLE ile Trafik Yoğunluğu Modellemesi
Proje Özeti
Bu projede, bir dakikada geçen araç sayıları kullanılarak trafik yoğunluğu Poisson dağılımı ile modellenmiştir. Amaç, dağılımın parametresi olan λ (lambda) değerini Maximum Likelihood Estimation (MLE) yöntemi ile tahmin etmektir.

Analiz hem teorik türetim hem de Python ile sayısal optimizasyon kullanılarak gerçekleştirilmiştir.

Veri
Analizde kullanılan araç sayıları:

Copy
[12, 15, 10, 8, 14, 11, 13, 16, 9, 12, 11, 14, 10, 15]
Bu değerler bir dakikalık zaman aralıklarında gözlemlenen araç sayısını temsil eder.

Yöntem
Poisson dağılımı için MLE sonucu:

λ̂ = (1/n) Σ k_i

Yani parametre tahmini veri ortalamasına eşittir.

Python tarafında ise negatif log‑likelihood fonksiyonu minimize edilerek aynı sonuç elde edilmiştir.

Sonuç
Yöntem	λ
Analitik MLE	12.14
Sayısal MLE	12.14
Ayrıca yapılan testte aykırı değerlerin MLE tahminini önemli ölçüde değiştirdiği görülmüştür.
