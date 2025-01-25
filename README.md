Akciğer Kanseri Tahmini Projesi Raporu
 Hazırlayan:
 ● EdaYamak

 1. Projenin Amacı
 Bu proje, akciğer kanseri risk faktörlerini analiz ederek bir bireyin akciğer kanseri olup
 olmadığını tahmin etmeyi amaçlamaktadır. Akciğer kanseri, erken teşhis edilmediğinde
 ölümcül sonuçlara yol açabilen ciddi bir hastalıktır. Bu projede, bir veri bilimi yaklaşımı
 kullanılarak çeşitli bireysel faktörlerin etkisi incelenmiş ve bir makine öğrenimi modeli ile
 akciğer kanseri tahmini yapılmıştır.
 2. Kullanılan Yöntemler
 2.1. Veri Hazırlığı
 Veri seti, toplamda 309 satır ve 16 sütun içermektedir. Sütunlar, bireylerin cinsiyet, yaş,
 sigara kullanımı, nefes darlığı gibi faktörlerini ve akciğer kanseri durumunu temsil etmektedir.
 Şu adımlar uygulanmıştır:
 ● EksikveTekrarlayan Veriler: Veri setindeki tekrar eden 33 satır kaldırılmış ve
 toplam 276 benzersiz kayıt elde edilmiştir.
 ● Etiketleme: Nitel veriler sayısal verilere dönüştürülmüştür (Evet = 1, Hayır = 0; Erkek
 = 1, Kadın = 0).
 2.2. Keşfisel Veri Analizi (EDA)
 Bağımsız değişkenlerin hedef değişkenle olan ilişkileri analiz edilmiş ve şu bulgular elde
 edilmiştir:
 ● Kronik hastalıklar, sarı parmak, kaygı ve göğüs ağrısı gibi faktörlerin akciğer kanseri
 ile anlamlı ilişkisi bulunmuştur.
 ● Sigara kullanımı ve yaş gibi faktörlerin doğrudan bir etkisi olmadığı görülmüştür.
 2.3. Veri Dengeleme
 Veri setindeki sınıf dengesizliğini azaltmak için ADASYN algoritması kullanılmış ve toplamda
 482 kayıt içeren dengeli bir veri seti elde edilmiştir.
 2.4. Modelleme
 ● Veri seti, bağımlı (LUNG_CANCER) ve bağımsız değişkenlere ayrılmıştır.
● Veriler %75 eğitim, %25 test olacak şekilde bölünmüştür.
 ● Logistic Regression algoritması ile model kurulmuş ve test verileri ile tahminler
 yapılmıştır.
 3. Sonuçlar
 ● Model, akciğer kanseri tahmini yaparken genel olarak düzgün bir performans
 sergilemiştir.
 ● Logistic Regression modeli kullanılarak test seti üzerinde %85 doğruluk oranı elde
 edilmiştir.
