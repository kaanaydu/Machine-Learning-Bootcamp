https://www.kaggle.com/code/kaanayduvann/churn-analysis-and-anomaly-dedection-of-googleapps

Not: Düzenlemeye girdiğinizde daha rahat okuyacaksınız.


Seçtiğimiz veri seti Google Play Store Apps ve şu sütunları içeriyor:

   App Name : Uygulamarın ismini içerir.
   App Id   : Uygulamaların eşşiz değerlerini içerir.
   Category : Uygulamarın kategorilerini belirtir.
   Rating   : Uygulamaların almış olduğu oylama puanını 1 ile 5 arasında gösterir.
   Rating Count : Uygulamarın kaç kez oylandığını gösterir.
   Installs : Uygulamaların indirilme sayısını gösterir.
   Minimum Installs : Uygulamaların minimum indirilme sayısını belirtir.
   Maximum Installs : Uygulamaların maksimum indirilme sayısını belirtir.
   Free : Uygulamaların ücretsiz olup olmadığını, true false şeklinde gösterir.
   Price : Uygulamaların ücretlerini gösterir.
   Currency : Uygulamalar ücretli ise para birimini belirtir.
   Size : Uygulamaların boyutunu gösterir.
   Minimum Android : Uygulamaların desteklediği minimum android sürümünü belirtir.
   Developer Id : Geliştiricinin kimliğini belirtir.
   Developer Website : Geliştiricinin sitesini gösterir.
   Developer Email : Geliştiricinin mail adresini gösterir.
   Released : Uygulamaların yayınlanma tarihini gösterir.
   Privacy Policy : Uygulamaların gizlilik politikası hakkında bilgi verir.
   Last Updated : Uygulamaların son güncellenme aldığı tarihi belirtir.
   Content Rating : Uygulamaların içeriğinin hangi kitleye yönelik olduğunu belirtir.
   Ad Supported : Uygulamaların reklamları destekleyip desteklemediğini true false şeklinde gösterir.
   In app purchases : Uygulama içi satın alım olup olmamasını true false şeklinde gösterir.
   Editors Choice : Editörler tarafından önerilip önerilmediğini gössterir.

Projelerimizde şu sütunları kullandık:
  App Name
  Rating
  Rating Count
  Installs
  Price
  Category
  Last Updated
  Free

  Churn Analysis projemizin final çıktısı:
  Mean Squared Error (MSE): 0.005553778039120735
  Mean Absolute Error (MAE): 0.005553778039120735
  Confusion Matrix:
      [[246653    663]
       [  1906 213346]]
  Accuracy: 0.9944462219608793
  Precision: 0.9969019994486213
  Recall: 0.9911452622972144
  F1: 0.9940152960553137

Noise and Anomaly Detection projemizin final çıktısı:
  Davies-Bouldin Skoru: 12.782790832582085
  Bu projenin değerlendirilmesi için değerlendirmesi için Davies Bouldin seçtik. Davies-Bouldin indeksi, bir kümeleme algoritmasının performansını değerlendirmek 
  için kullanılan bir ölçüttür. Davies-Bouldin indeksi, her bir kümenin merkezinden (veya ortalama noktası) uzaklık ile o kümedeki örneklerin birbirine ne kadar      yakın olduğuna bakar.


Veri setimizde, Google Play Store'daki Android uygulamalarının kategorilerini tahmin etmek için denetimli öğrenme yöntemlerinden sınıflandırma algoritmalarının kullanımına son derece uygundur. Her uygulamanın sahip olduğu "Kategori" etiketi, bu verinin model eğitimi için ideal bir temel sunar. Sınıflandırma algoritmaları arasında Lojistik Regresyon, Doğrusal Regresyon gibi seçenekler bulunmaktadır. Bu algoritmalar, verinin karmaşıklığı, boyutu, hesaplama gücü ve istenen doğruluk düzeyine bağlı olarak değişkenlik gösterir.

Uygun algoritmanın belirlememiz, deneysel bir yaklaşım gerektirdi. Bu nedenle farklı algoritmaları test ederek performanslarını karşılaştırarak sonuçları gözlemledik. Özellik mühendisliği, modelin doğruluğunu artırmak için önemli bir adım olup, özelliklerin anlamlı hale getirilmesiyle modelin genel başarısı artırılabilir. Ayrıca, model değerlendirme metrikleri ve aşırı öğrenmeyi önlemek için düzenleme teknikleri gibi yöntemlerin kullanılması, daha iyi sonuçlar elde edilmesini sağlayacaktır.
