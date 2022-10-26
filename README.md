# Denetimli_-rneme_Regresyon
Denetimli öğrenme algoritmaları : regresyon ( basit doğrusal regresyon ve çoklu regresyon) kullanım alanları ve örnekleri
Deneyimli öğrneme nedir
Denetimli öğrenme; aldığı veriler ve ürettiği sonuçlara dayalı olarak bir model geliştirme işlemidir. Diğer makine öğrenmesi türlerine kıyasla denetimli öğrenmenin en büyük farkı veri etiketi kullanılmasıdır. Etiketlediğimiz veriye, gösterdiğimiz sınıf ve bilgiye göre mevcut gerçekliğe dayanarak model geliştirme algoritmasıdır.

Örnekler üzerinde bir öğrenme sağlar ve yeni girdilerde de etiketi tahmin etmeye çalışır.
Denetimli öğrenmede, makine, bir öğrenme algoritması aracılığıyla etiketli eğitim verilerini çalıştırarak, gelir ve eğitim arasındaki ilişkiyi sıfırdan öğrenmeye çalışır. Denetimli öğrenmenin amacı, Y’nin bilindiği ve Y’nin bilinmediği yeni örnekler verildiğinde Y’yi mümkün olduğunca doğru bir şekilde tahmin etmektir. 

Örnek verecek olursak:
Spam ya da spam olmayan mailleri ayırt etmek için elimizde bir veri seti olsun. Bu veri setini kullanarak bir model eğitme işlemi denetimli öğrenmedir.
Denetimli öğrenmenin tarihçesi
    Denetimli öğrenme fikri Perceptron deneyi ile ortaya çıkmıştır. Bu deneyle yapay sinir ağının temelleri atılmıştır. 
    1958 yılında psikolog Frank Rosenblatt tarafından üçgen ya da üçgen olmayan nesneleri belirlemek için bir çalışma yürütülüyor. Rosenblatt  zamanına göre yüksek kalitede kameralar(400 pixel) kullanarak oldukça büyük bir makine yapıyor ve buna da perceptron ismini veriyor. Perceptron tek katmanlı yapay sinir ağından oluşuyordu.
    Öğrenmeyi gerçekleştirmek için önce, kameraya çeşitli resimler gösteriyor. Deney için 2 sınıfımız var. Üçgen ya da değil.
    Kamera gördüğü şeye bağlı olarak perceptrona farklı bir elektrik sinyal gönderiyor. Daha sonra Rosenblatt, üçgen şekliyle eşleşen tüm sinyalleri perceptrona uyguluyor. Eğer total skor threshold değerinden büyükse makine bir elektrik sinyali gönderir ve ışıklar açılır. Eğer elektriksel yük threshold değerinden küçükse ışık yanmıyor ve bu da üçgen olmadığı anlamına geliyor. İlk başta perceptron rastgele tahminler yaparak threshold değerini belirlemek için kullanıldı.Daha sonra Rosenblatt ‘evet’, ‘hayır’ butonlarıyla denetimli öğrenmeyi gerçekleştirdi. Eğer perceptron doğru tahmin yapıyorsa ‘evet’ tuşuna basıyordu,yanlış tahminde de sinapslardan geçen elektrik değerini ölçüp threshold değeri olarak belirliyordu.
    Evet, hayır butonları kullanıldığı için, bu uygulama denetimli öğrenmenin temeli sayıldı.
 Regresyon nedir ?
 Regresyon, bir bağımlı değişken (genellikle Y ile gösterilir) ve diğer bağımsız değişkenler arasındaki ilişkinin gücünü ve karakterini belirlemeye çalışan finans, yatırım, makine öğrenmesi ve diğer disiplinlerde kullanılan istatistiksel bir yöntemdir.

Bağımlı Değişken: Anlamaya veya tahmin etmeye çalıştığımız değişkendir. 
Bağımsız Değişken: Analizi veya hedef değişkeni etkileyen ve değişkenlerin hedef değişkenle ilişkisi hakkında bize bilgi veren faktörlerdir.
Makıine öğrenmesinde regresyon
Makine öğrenmesinde regresyon ise kısaca makinenin veri setini ezberlememesi için oluşturulan algoritmadır. İstenen sonuç makinenin ezberlemesi değil “öğrenmesi” yani tutarlı tahmin yeteneğine sahip olmasıdır.
Yöntem olarak bir eğitim kümesi ve eğitim kümesinden makine öğrenmesi metotları ile bir model elde edilip bu model üzerinden yeni gelen veriler tahmin edilmeye çalışılır. Regresyon yönteminde tahmin sonucu kategorik değil nümerik bir değer olmalıdır. Örneğin: 
Kategorik tahmin sonucu: Hava çok soğuk, hava soğuk, hava ılık, hava sıcak, hava çok sıcak gibi. 
Nümerik tahmin sonucu: Hava -10 derece, 0 derece, 10.01 derece, 30.02 derece gibi sayısal değerlerdir.

Regresyon çeşitleri
Doğrusal Regresyon: Doğrusal regresyon, iki değişken arasındaki doğrusal ilişkinin bir doğru denklemi olarak tanımlanıp, değişkenin değerlerinden biri bilindiğinde diğeri hakkında tahmin yapılmasını sağlar.
doğrusal regresyon örneği
İş arkadaşlarınızın daha önce zaten anladıklarını görmüş ve düşünmüş olabilecekleri kalıpları ve ilişkileri ortaya çıkararak daha iyi iç görüler sağlamak için de doğrusal regresyondan yararlanabilirsiniz. Örneğin, satış ve satın alma verilerini analiz etmek, belirli günlerdeki ya da belirli saatlerdeki belirli satın alma kalıplarını ortaya çıkarmanıza yardımcı olabilir. Regresyon analizinden toplanan iç görüler, iş liderlerinin şirketlerinin ürünlerinin yüksek talep göreceği zamanları tahmin etmelerine yardımcı olabilir.
Doğrusal regresyon, basit doğrusal regresyon ve çoklu doğrusal regresyon olarak iki başlık altında incelenir.
Basit doğrusal regresyon, yanıt değişkeni ile tek bir açıklayıcı değişken arasındaki doğrusal ilişkiyi açıklar. Eğer tek bir yanıt değişkeni ve birden fazla açıklayıcı değişken arasındaki doğrusal veya eğrisel bir ilişki tanımlanmak istenirse, ilişki çoklu doğrusal regresyon ile incelenir (Okur, 2009; Weisberg, 2005).
2-Polinom Regresyon: Bir bağımlı ve birden fazla bağımsız değişken arasında polinomyal bir artış söz konusu ise bu algoritmayı kullanırız. Polinom Regresyon Formülü: 
Y = a + bX + cX²
3– Karar Ağacı Regresyonu: Karar Ağaçları Algoritmaları hem sınıflandırma da hem de regresyonda kullanılır. Regresyon için kullanılan algoritmayı şöyle açıklayabiliriz; Bağımsız değişkenleri bilgi kazancına göre aralıklara ayırır. Tahmin esnasında bu aralıktan bir değer sorulduğunda cevap olarak bu aralıktaki (eğitim esnasında öğrendiği) ortalamayı verir. Belli aralıklarda istenilen değerler için aynı sonuçları ürettiğinden kesikli bir modeldir.
4-Lojistik Regresyon: Lojistik regresyon, istatistikte kullanılan bir model oluşturma tekniği olup iki ya da daha fazla sınıfta ifade edilebilen kesikli verilerde yanıt değişkeni (Y) için bir model oluşturma tekniğidir.
Örneğin, web sitesi ziyaretçinizin alışveriş sepetindeki ödeme düğmesine tıklayıp tıklamayacağını tahmin etmek istediğinizi varsayalım. Lojistik regresyon analizi, web sitesinde harcanan zaman ve sepetteki ürün sayısı gibi geçmiş ziyaretçi davranışlarına bakar. Geçmişte, ziyaretçiler sitede beş dakikadan fazla zaman geçirdiyse ve sepete üçten fazla ürün eklediyse ödeme düğmesine tıkladıklarını belirler. Lojistik regresyon işlevi bu bilgiyi kullanarak daha sonra yeni bir web sitesi ziyaretçisinin davranışını tahmin edebilir.
BASİT DOĞRUSAL REGRESYON
Açıklayan(bağımlı) ile  tek bir açıklayıcı (bağımsız) değişkenin arasındaki doğrusal ilişkinin modellenmesidir. Bir başka ifadeyle bağımlı değişkenin değerini bağımsız denklemin bir fonksiyonu olarak en doğru şekilde tahmin eden doğrusal ilişkidir. Burada tahmin edilmek istenen bağımlı değişkendir.
İki değişken arasındaki ilişkinin ne kadar güçlü olduğu
Bağımsız değişkenin belirli bir değerinde bağımlı değişkenin değeri
Bilgilerine ulaşmak için basit doğrusal regresyon kullanılır.
Gelir ve mutluluk arasındaki ilişkiyle ilgilenen bir araştırmacı olduğunuzu düşünün. Gelirleri 15 bin ile 75 bin arasında değişen 500 kişiyi araştırıyorsunuz ve onlardan mutluluklarını 1'den 10'a kadar puanlamalarını istiyorsunuz.
Bağımsız değişkeniniz (gelir) ve bağımlı değişkeniniz (mutluluk) niceldir, bu nedenle aralarındaki ilişkiyi basit doğrusal regresyon analizi ile açıklayabilirsiniz.

Basit Doğrusal Regresyon  Hesaplamaları
𝓎 = ß0+ß1X+𝑒
𝓎 = yanıt değişkeni
ß0 = kesim noktası
ß1 = doğrunun eğimi
X = bağımsız değişken
𝑒 = hata payı(kalıntı)

𝓔 Nedir?
Gerçek değer ve tahmini değer arasındaki farktır.
Bu farka göre modeller arasındaki doğruluk kontrolü yapılır.


	𝓔i = yi - ŷi

	yi = gerçek değer
 
	ŷi  = tahmini çıktı
  
  Basit doğrusal regresyon analizi sonucu parametre kestirimlerinin güvenli olabilmesi için bazı varsayımların geçerli olması gereklidir .
Modeldeki bağımsız değişkenlerin, bağımlı değişkeni ne kadar açıkladığı R2 değeri ile ölçülür.
R2 değerini hesaplamak için 
Toplam Kareler Toplamı
Artık Kareler Toplamı
değerlerine ihtiyaç duyarız. R2  0-1 arasında bir değer alır. R2 değerinin 1’e yakın olması bağımsız değişkenlerin, bağımlı değişkenleri iyi bir şekilde açıkladığını gösterir.
ÇOKLU REGRESYON
Doğrusal regresyon bir bağımsız değişkenin bir bağımlı değişken üzerine etkisini göstermeye yararken, çoklu regresyonda bağımsız değişken sayısı birin üstüne çıkar. 
En az iki bağımsız değişkenin, bağımlı değişken üzerinde etkilerini göstermeye yarayan analiz yöntemidir.
İki değişken varsa, tahminin temelini oluşturan değişken bağımsız değişkendir. Değeri tahmin edilecek değişken bağımlı değişken olarak bilinir

Çoklu Regresyon Nedir?
Çoklu lineer regresyonda her bağımsız değişkenin bağımlı değişkene etkime derecesi birbirinden farklıdır. Bundan dolayı basit lineer regresyondaki denkleme ek olarak her değişkenin katsayısı aynı olmak zorunda değildir. 

P Değeri Nedir?
P değeri, bizim hipotezlerimizin doğru olup olmadığını belirlememize yardımcı olan istatistiksel bir ölçüdür.
P değerleri, deney sonuçlarının gözlemlenen olaylar için normal değerler aralığında olup olmadığını belirlemek için kullanılır. 
Genellikle, bir veri setinin P değeri önceden belirlenmiş belirli bir miktarın altındaysa (örneğin, 0.05 gibi), bilim insanları deneylerinin "boş hipotezini" reddedeceklerdir.
Yani ilgili değişkenin sonuç üzerinde anlamlı bir etkisinin olmadığı anlaşılır.

