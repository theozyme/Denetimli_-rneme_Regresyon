# Denetimli öğrenme algoritmaları : regresyon ( basit doğrusal regresyon ve çoklu regresyon) kullanım alanları ve örnekleri
## Deneyimli öğrneme nedir
Denetimli öğrenme; aldığı veriler ve ürettiği sonuçlara dayalı olarak bir model geliştirme işlemidir. Diğer makine öğrenmesi türlerine kıyasla denetimli öğrenmenin en büyük farkı veri etiketi kullanılmasıdır. Etiketlediğimiz veriye, gösterdiğimiz sınıf ve bilgiye göre mevcut gerçekliğe dayanarak model geliştirme algoritmasıdır.

Örnekler üzerinde bir öğrenme sağlar ve yeni girdilerde de etiketi tahmin etmeye çalışır.
Denetimli öğrenmede, makine, bir öğrenme algoritması aracılığıyla etiketli eğitim verilerini çalıştırarak, gelir ve eğitim arasındaki ilişkiyi sıfırdan öğrenmeye çalışır. Denetimli öğrenmenin amacı, Y’nin bilindiği ve Y’nin bilinmediği yeni örnekler verildiğinde Y’yi mümkün olduğunca doğru bir şekilde tahmin etmektir. 

### Örnek verecek olursak:
Spam ya da spam olmayan mailleri ayırt etmek için elimizde bir veri seti olsun. Bu veri setini kullanarak bir model eğitme işlemi denetimli öğrenmedir.
## Denetimli öğrenmenin tarihçesi
Denetimli öğrenme fikri Perceptron deneyi ile ortaya çıkmıştır. Bu deneyle yapay sinir ağının temelleri atılmıştır. 
1958 yılında psikolog Frank Rosenblatt tarafından üçgen ya da üçgen olmayan nesneleri belirlemek için bir çalışma yürütülüyor. Rosenblatt  zamanına göre yüksek kalitede kameralar(400 pixel) kullanarak oldukça büyük bir makine yapıyor ve buna da perceptron ismini veriyor. Perceptron tek katmanlı yapay sinir ağından oluşuyordu.
Öğrenmeyi gerçekleştirmek için önce, kameraya çeşitli resimler gösteriyor. Deney için 2 sınıfımız var. Üçgen ya da değil.
Kamera gördüğü şeye bağlı olarak perceptrona farklı bir elektrik sinyal gönderiyor. Daha sonra Rosenblatt, üçgen şekliyle eşleşen tüm sinyalleri perceptrona uyguluyor. Eğer total skor threshold değerinden büyükse makine bir elektrik sinyali gönderir ve ışıklar açılır. Eğer elektriksel yük threshold değerinden küçükse ışık yanmıyor ve bu da üçgen olmadığı anlamına geliyor. İlk başta perceptron rastgele tahminler yaparak threshold değerini belirlemek için kullanıldı.Daha sonra Rosenblatt ‘evet’, ‘hayır’ butonlarıyla denetimli öğrenmeyi gerçekleştirdi. Eğer perceptron doğru tahmin yapıyorsa ‘evet’ tuşuna basıyordu,yanlış tahminde de sinapslardan geçen elektrik değerini ölçüp threshold değeri olarak belirliyordu.
    Evet, hayır butonları kullanıldığı için, bu uygulama denetimli öğrenmenin temeli sayıldı.
 ## Regresyon nedir ?
 Regresyon, bir bağımlı değişken (genellikle Y ile gösterilir) ve diğer bağımsız değişkenler arasındaki ilişkinin gücünü ve karakterini belirlemeye çalışan finans, yatırım, makine öğrenmesi ve diğer disiplinlerde kullanılan istatistiksel bir yöntemdir.

**Bağımlı Değişken**: Anlamaya veya tahmin etmeye çalıştığımız değişkendir. 
**Bağımsız Değişken**: Analizi veya hedef değişkeni etkileyen ve değişkenlerin hedef değişkenle ilişkisi hakkında bize bilgi veren faktörlerdir.
## Makine öğrenmesinde regresyon
Makine öğrenmesinde regresyon ise kısaca makinenin veri setini ezberlememesi için oluşturulan algoritmadır. İstenen sonuç makinenin ezberlemesi değil “öğrenmesi” yani tutarlı tahmin yeteneğine sahip olmasıdır.
Yöntem olarak bir eğitim kümesi ve eğitim kümesinden makine öğrenmesi metotları ile bir model elde edilip bu model üzerinden yeni gelen veriler tahmin edilmeye çalışılır. Regresyon yönteminde tahmin sonucu kategorik değil nümerik bir değer olmalıdır. Örneğin: 
**Kategorik tahmin sonucu**: Hava çok soğuk, hava soğuk, hava ılık, hava sıcak, hava çok sıcak gibi. 
**Nümerik tahmin sonucu**: Hava -10 derece, 0 derece, 10.01 derece, 30.02 derece gibi sayısal değerlerdir.

## Regresyon çeşitleri
### **Doğrusal Regresyon**:
Doğrusal regresyon, iki değişken arasındaki doğrusal ilişkinin bir doğru denklemi olarak tanımlanıp, değişkenin değerlerinden biri bilindiğinde diğeri hakkında tahmin yapılmasını sağlar.
### doğrusal regresyon örneği
İş arkadaşlarınızın daha önce zaten anladıklarını görmüş ve düşünmüş olabilecekleri kalıpları ve ilişkileri ortaya çıkararak daha iyi iç görüler sağlamak için de doğrusal regresyondan yararlanabilirsiniz. Örneğin, satış ve satın alma verilerini analiz etmek, belirli günlerdeki ya da belirli saatlerdeki belirli satın alma kalıplarını ortaya çıkarmanıza yardımcı olabilir. Regresyon analizinden toplanan iç görüler, iş liderlerinin şirketlerinin ürünlerinin yüksek talep göreceği zamanları tahmin etmelerine yardımcı olabilir.
Doğrusal regresyon, basit doğrusal regresyon ve çoklu doğrusal regresyon olarak iki başlık altında incelenir.
Basit doğrusal regresyon, yanıt değişkeni ile tek bir açıklayıcı değişken arasındaki doğrusal ilişkiyi açıklar. Eğer tek bir yanıt değişkeni ve birden fazla açıklayıcı değişken arasındaki doğrusal veya eğrisel bir ilişki tanımlanmak istenirse, ilişki çoklu doğrusal regresyon ile incelenir (Okur, 2009; Weisberg, 2005).
### Polinom Regresyon:
Bir bağımlı ve birden fazla bağımsız değişken arasında polinomyal bir artış söz konusu ise bu algoritmayı kullanırız. Polinom Regresyon Formülü: 
Y = a + bX + cX²
### Karar Ağacı Regresyonu: Karar Ağaçları Algoritmaları hem sınıflandırma da hem de regresyonda kullanılır. Regresyon için kullanılan algoritmayı şöyle açıklayabiliriz; Bağımsız değişkenleri bilgi kazancına göre aralıklara ayırır. Tahmin esnasında bu aralıktan bir değer sorulduğunda cevap olarak bu aralıktaki (eğitim esnasında öğrendiği) ortalamayı verir. Belli aralıklarda istenilen değerler için aynı sonuçları ürettiğinden kesikli bir modeldir.
### Lojistik Regresyon: Lojistik regresyon, istatistikte kullanılan bir model oluşturma tekniği olup iki ya da daha fazla sınıfta ifade edilebilen kesikli verilerde yanıt değişkeni (Y) için bir model oluşturma tekniğidir.
Örneğin, web sitesi ziyaretçinizin alışveriş sepetindeki ödeme düğmesine tıklayıp tıklamayacağını tahmin etmek istediğinizi varsayalım. Lojistik regresyon analizi, web sitesinde harcanan zaman ve sepetteki ürün sayısı gibi geçmiş ziyaretçi davranışlarına bakar. Geçmişte, ziyaretçiler sitede beş dakikadan fazla zaman geçirdiyse ve sepete üçten fazla ürün eklediyse ödeme düğmesine tıkladıklarını belirler. Lojistik regresyon işlevi bu bilgiyi kullanarak daha sonra yeni bir web sitesi ziyaretçisinin davranışını tahmin edebilir.
# BASİT DOĞRUSAL REGRESYON
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
# ÇOKLU REGRESYON
Doğrusal regresyon bir bağımsız değişkenin bir bağımlı değişken üzerine etkisini göstermeye yararken, çoklu regresyonda bağımsız değişken sayısı birin üstüne çıkar. 
En az iki bağımsız değişkenin, bağımlı değişken üzerinde etkilerini göstermeye yarayan analiz yöntemidir.
İki değişken varsa, tahminin temelini oluşturan değişken bağımsız değişkendir. Değeri tahmin edilecek değişken bağımlı değişken olarak bilinir

##Çoklu Regresyon Nedir?
Çoklu lineer regresyonda her bağımsız değişkenin bağımlı değişkene etkime derecesi birbirinden farklıdır. Bundan dolayı basit lineer regresyondaki denkleme ek olarak her değişkenin katsayısı aynı olmak zorunda değildir. 

### P Değeri Nedir?
P değeri, bizim hipotezlerimizin doğru olup olmadığını belirlememize yardımcı olan istatistiksel bir ölçüdür.
P değerleri, deney sonuçlarının gözlemlenen olaylar için normal değerler aralığında olup olmadığını belirlemek için kullanılır. 
Genellikle, bir veri setinin P değeri önceden belirlenmiş belirli bir miktarın altındaysa (örneğin, 0.05 gibi), bilim insanları deneylerinin "boş hipotezini" reddedeceklerdir.
Yani ilgili değişkenin sonuç üzerinde anlamlı bir etkisinin olmadığı anlaşılır.
## Çoklu Lineer Regresyon Modeli Oluşturmak
Çoklu lineer regresyon modeli oluştururken oldukça fazla parametrenin dikkatle incelenmesi gerekir, çünkü her bir değerin bağımlı değişken üzerinde anlamlı bir etkisi olmayabilir. 
Bağımlı değişkeni yüksek oranda etkileyen bir değişkeni veri setinden kaldırdığımız zaman oluşacak hatalar veya gereksiz bir değişkeni veri setinden atmadığımız zaman kaybedeceğimiz verim istenilmeyen bir sonuçtur.
Bu durumu doğru şekilde incelemek için belirli istatistik modelleri vardır. 
## Regresyon Modeli Kurulumunda 5 Metod
**Bağımsız değişkenlerin hepsini birden modele dahil etmek (All-in)**
**Geriye doğru eleme (Backward Elimination)**
**İleriye doğru seçme (Forward Selection):**
**İki yönlü eleyerek seçme (Bidirectional Elimination)**
**Sonuçları karşılaştırma (Score comparision)**
## Geriye Doğru Eleme
Geriye doğru eleme yöntemi tüm değişkenleri içeren bir modelden, fazlalıklarını atarak daha verimli daha küçük bir model oluşturma içeren algoritmadır.
Değişkenlerin modelde kalması için önem değeri belirlenir. Bir çeşit eşik değeri(threshold) olarak işlev görür. (p<0.05) 
Modelle alakasız değişkenler modelden çıkarılır.
En yüksek P değerine sahip değişkeni bul. Eğer önem değerinden yüksekse (P>SL) bir sonraki adıma ilerle. Eğer düşükse modelin geriye doğru eleme algoritmasını tamamlamıştır.
P değeri önem değerinden yüksek değişkeni modelden çıkart ve 3. adıma dön.
## Regresyon Analizi Nasıl Yapılır?Çalışma Mantığı Nedir ?
### Bir Hipotez Oluşturulur 
 Bir regresyon analizi yapmak için, ilişkili olduğuna inandığınız iki değişkeni seçmeniz gerekir. Mümkün olduğu kadar çok veri toplayarak ilişkileri hakkında hipotezinizi oluşturun. Reklam ve satış ilişkisi söz konusu olduğunda, daha doğru bir analiz için bir yıl boyunca oluşan tüm finansal verileri toplayabilirsiniz.
### Bir Grafik Oluşturulur
Bir sonraki adım, verilerinizin grafiğini çıkarmaktır. İki veri seti ile doğrusal regresyon için temel bir çizgi grafiği oluşturabilirsiniz. Bir değişken X ekseninde, diğeri Y ekseninde çizilir. Bir elektronik tabloya girdiğinizde, değişkenler arasındaki korelasyonu görebilirsiniz. Düz bir çizgi varsa, bu pozitif bir korelasyon gösterir.
![image](https://user-images.githubusercontent.com/71380452/198358700-48270dd1-2ae8-4d1d-8a81-98bbf6635633.png)
### . Sonuçlar Analiz Edilir.
Grafiği temel bir doğrusal regresyonda inceleyerek kesişim, katsayı ve korelasyonu görebilirsiniz. Bu rakamları bir araya getirmek, iki veri seti arasındaki tarihsel ilişkiyi göstererek modelin gelecekte nasıl görüneceğini tahmin etmenize olanak tanır. Geçmişte, çevrimiçi reklamcılık ve satışlar arasında olumlu bir ilişki varsa, gelecek yıl için bir tahmin oluşturmak için yüzdeleri bir modele ekleyebilirsiniz. 
![image](https://user-images.githubusercontent.com/71380452/198358871-2a7f0da9-7aaf-41cc-82c7-46f18e209f80.png)
# Regresyon Analizi Kullanım Alanları
**Tahmin**
![image](https://user-images.githubusercontent.com/71380452/198359138-f6558cf4-fea2-4587-9c6b-1acab79d3c32.png)
**CAPM**
Bir varlığın öngörülen getirisi ile ilgili piyasa risk primi arasındaki bağlantıyı kuran The Capital Asset Pricing Model (CAPM), doğrusal regresyon modeline dayanır. Ayrıca, kurumsal getirileri ve operasyonel performansı tahmin etmek için finansal analistler tarafından finansal analizde sıklıkla kullanılır.
Bir hisse senedinin beta katsayısı, regresyon analizi kullanılarak hesaplanır. Beta, toplam piyasa riskiyle ilgili getiri oynaklığının bir ölçüsüdür.
**Rekabet karşılaştırma**
Bir şirketin finansal performansını belirli bir muadili ile karşılaştırmak için kullanılabilir. Ayrıca iki firmanın hisse senedi fiyatları arasındaki ilişkiyi belirlemek için de kullanılabilir ve hangi yönlerin satışlarını etkilediğini belirlemede firmaya yardımcı olabilir. Bu teknikler, küçük işletmelerin kısa sürede hızlı başarıya ulaşmalarına yardımcı olabilir.
# Regresyon Analizi Hangi Sektörlerde Var?
Finans Sektörü: 
Finansta, bir hisse senedinin BETA’sını hesaplamak için regresyon analizi kullanılır. Üstelik bunu Excel yardımı ile kolayca yapabilirsiniz.
Yine finansta, şirketler için mali tabloları tahmin etmek için regresyon analizi de kullanılır. Böylece, iş varsayımlarındaki hangi değişikliklerin gelecekteki giderleri ve geliri etkileyeceğini belirleyebilirsiniz.
Bir şirketin satışları son birkaç yıldır her ay istikrarlı bir şekilde arttıysa, satış verileri üzerinde aylık satışlarla doğrusal bir analiz yaparak şirketin gelecek aylardaki satışlarını tahmin edebilirsiniz.
Bir firmanın yöneticisi, gelecek planlaması için reklam harcamaları ile satışlar arasındaki kesin ilişkiyi öğrenmek istiyorsa, regresyon tekniği ile bu ilişkiyi tahmin edebilir.
Pazarlama:
 Pazar kampanyalarının etkinliğini, tahmin fiyatlandırmasını ve ürünün satışını anlamak.
Üretim:
 Daha iyi performans sağlamak için değişkenlerin ilişkisini değerlendirmek.
İlaç:
 Hastalıklar için jenerik ilaçlar hazırlamak için farklı ilaç kombinasyonlarını tahmin etmek.
# Basit Doğrusal Ve Çoklu Regresyon Örnekleri
İşletmeler, reklam harcamaları ile gelir arasındaki ilişkiyi anlamak için genellikle doğrusal regresyon kullanır.
# örnekler
İşletmeler, reklam harcamaları ile gelir arasındaki ilişkiyi anlamak için genellikle doğrusal regresyon kullanır.

![image](https://user-images.githubusercontent.com/71380452/198360016-2f63c8ec-18ae-4410-8363-149531938cb7.png)
Tıbbi araştırmacılar, ilaç dozu ile hastaların kan basıncı arasındaki ilişkiyi anlamak için sıklıkla doğrusal regresyon kullanırlar.
![image](https://user-images.githubusercontent.com/71380452/198360285-45c1640c-e054-48ea-9595-26bd49437059.png)
Tarım bilimcileri, gübre ve suyun mahsul verimi üzerindeki etkisini ölçmek için genellikle doğrusal regresyon kullanırlar.
![image](https://user-images.githubusercontent.com/71380452/198360446-9b42f58b-38ff-453b-bc3a-81e015d518d1.png)
![image](https://user-images.githubusercontent.com/71380452/198360486-69bd505f-24c5-4c75-9d00-5074aee2acc1.png)
### Gayrimenkul Örneği
Ev satmak için en iyi zamanı tahmin etmeye yardımcı olacak bir model oluşturmak isteyen bir emlak uzmanısınız. Evleri maksimum satış fiyatından satmak istersiniz, ancak satış fiyatını birden fazla faktör etkileyebilir. Bu değişkenler, diğer faktörlerin yanı sıra evin yaşını, mahalledeki diğer evlerin değerini, devlet okulu sisteminin öğrenci performansına ilişkin nicel ölçümlerini ve yakındaki parkların sayısını içerir.Evlerin maksimum satış fiyatını tahmin etmek için bu dört bağımsız değişkenden bir tahmin modeli oluşturabilirsiniz. Bu faktörlerden herhangi biri katsayı değerleri açısından değişirse değişkenleri ayarlayabilirsiniz.
### İş Örneği
Halka açık bir şirkette hisse senediniz var ve şimdi hisse senedinizi satmak için iyi bir zaman olup olmayacağını bilmek istiyorsunuz. Şirketin karlılığı, şirketin maliyetleri, şirketin rekabeti ve şirketin varlıkları dahil olmak üzere hisse senedi fiyatının değerini çeşitli değişkenler etkileyebilir. Hisse senedini hemen satmanız mı yoksa hisse senedini elinde tutmaya devam etmeniz mi gerektiğine karar vermenize yardımcı olmak için bu dört bağımsız değişkenden bir tahmin modeli oluşturabilirsiniz
### Halk Sağlığı Örneği
Bulaşıcı bir hastalığın yayılmasını inceleyen bir epidemiyologsunuz. Mevcut bilinen enfeksiyonlara dayanarak bu hastalığın gelecekteki yayılmasını tahmin etmek istiyorsunuz. Çok sayıda bağımsız değişken, popülasyon büyüklüğü, popülasyon yoğunluğu, hava sıcaklığı, asemptomatik taşıyıcılar ve popülasyonun sürü bağışıklığına ulaşıp ulaşmadığı dahil olmak üzere gelecekteki enfeksiyonların sayısını etkileyebilir. Yordayıcı değişkenlerin katsayı değerlerindeki olası değişiklikleri hesaba katan bir sonucu tahmin etmek için ampirik veriler üzerinde istatistiksel modelleme ve çoklu doğrusal regresyon analizi yapabilirsiniz.

