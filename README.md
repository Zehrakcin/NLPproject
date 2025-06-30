

Bu proje, farklı kategorilere ait Türkçe haber metinlerini makine öğrenmesi yöntemleriyle sınıflandırmayı amaçlamaktadır. Metin önişlemeden sonra TF-IDF vektörleştirme uygulanmış, Naive Bayes ve SVM algoritmaları ile sınıflandırılmıştır. Ayrıca, TF-IDF vektörleri PCA ile iki boyuta indirgenerek görselleştirilmiştir.

---

## Kullanılan Teknolojiler ve Kütüphaneler

- Python
- Pandas, NumPy
- Scikit-learn (TF-IDF, PCA, Naive Bayes)
- NLTK (tokenization, stopword removal)
- SnowballStemmer (Turkish)
- Matplotlib (görselleştirme)

---

##  Uygulanan Adımlar

1. Veri Yükleme: `data.csv` dosyasındaki haber metinleri yüklendi.
2. Metin Temizleme:
   - Noktalama işaretleri kaldırıldı.
   - Küçük harfe çevirme uygulandı.
   - Stopwords temizliği yapıldı.
   - Türkçe kök bulma (stemming) uygulandı.
3. Vektörleştirme:
   - Her kategori için ayrı ayrı TF-IDF vektörleri çıkarıldı.
4. Görselleştirme:
   - TF-IDF vektörleri PCA ile 2 boyuta indirildi.
   - Her sınıf için ayrı renklerde scatter plot çizildi.
5. Modelleme:
   - Naive Bayes ve SVM modeli eğitildi ve test edildi.
