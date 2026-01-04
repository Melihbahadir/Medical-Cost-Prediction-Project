#  Medical Cost Prediction Project (Sağlık Sigortası Masraf Tahmini)

Merhaba! Bu repo, **Veri Analizi dersi dönem projesi** kapsamında hazırladığım makine öğrenmesi çalışmasını içermektedir.

Bu projede, bireylerin kişisel özelliklerine (yaş, vücut kitle indeksi, sigara kullanımı vb.) bakarak yıllık sağlık sigortası masraflarını tahmin eden bir model geliştirdim.

##  Projenin Amacı
Ders boyunca öğrendiğimiz veri analizi, veri ön işleme ve makine öğrenmesi tekniklerini gerçek bir veri seti üzerinde uygulamak ve **Regresyon (Tahminleme)** başarısı yüksek bir model ortaya çıkarmaktır.

##  Veri Seti
Projede Kaggle üzerinde bulunan popüler **"Medical Cost Personal Datasets"** verisini kullandım.
* **Veri Kaynağı:** [Kaggle Linki](https://www.kaggle.com/code/bahadiribik/medical-cost-personal-datasets)
* **Veri İçeriği:** Yaş, Cinsiyet, BMI (Vücut Kitle İndeksi), Çocuk Sayısı, Sigara Kullanımı, Bölge ve Masraflar (Charges).

##  Neler Yaptım? (Proje Adımları)

Projeyi geliştirirken şu adımları izledim:

1.  **Veri Keşfi (EDA):** Veriyi analiz ettim. Özellikle **sigara kullanımı** ve **BMI** değerlerinin masraflar üzerinde çok büyük bir etkisi olduğunu grafiklerle görselleştirdim.
2.  **Veri Ön İşleme:** Makine öğrenmesi algoritmalarının çalışabilmesi için kategorik verileri (Kadın/Erkek, Sigara Evet/Hayır gibi) sayısal değerlere dönüştürdüm (**Label Encoding**).
3.  **Model Kurulumu:** Bu bir regresyon problemi olduğu için, karmaşık ilişkileri daha iyi yakalayan **Random Forest Regressor** algoritmasını tercih ettim.
4.  **Model Eğitimi:** Veriyi %80 Eğitim, %20 Test olacak şekilde ayırdım ve modelimi eğittim.

##  Elde Ettiğim Sonuçlar

Test verisi üzerinde yaptığım değerlendirmeler sonucunda modelim oldukça başarılı sonuçlar verdi:

* **R2 Score (Başarı Oranı):** 0.86 (%86)
* **Temel Bulgum:** Sigorta masrafını belirleyen en kritik faktörün, kişinin sigara içip içmemesi olduğunu tespit ettim.

##  Kullanılan Teknolojiler
Bu projeyi hazırlarken aşağıdaki Python kütüphanelerinden yararlandım:
* **Pandas & NumPy:** Veri işleme ve manipülasyon.
* **Matplotlib & Seaborn:** Veri görselleştirme.
* **Scikit-learn:** Model kurulumu, eğitim ve değerlendirme metrikleri.

---
*Bu proje Veri Analizi dersi final ödevi için Melih Bahadır Şibik tarafından hazırlanmıştır.*
