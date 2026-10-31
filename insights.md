# PayFlow SQL Insights

## Question 1

**Business Question:** PayFlow veri setinde toplam kaç işlem bulunmaktadır?

**Result:** 1.200 toplam kayıt.

**Insight:** Veri setinde 1.200 ödeme denemesi bulunmaktadır. Bu değer, projedeki sonraki tüm analizlerin ve oranlamaların temel işlem bazını oluşturur.

---

## Question 2

**Business Question:** Başarılı işlemlerin ortalama işlem tutarı nedir?

**Result:** Başarılı statüdeki işlemlerin ortalama tutarı listelenmiştir.

**Insight:** Başarılı ödemelerin ortalama sepet büyüklüğünü görmek için bir baz oluşturur; ancak tek başına tüm müşteri segmentlerinin ve kategorilerin harcama davranışını yansıtmaz.

---

## Question 3

**Business Question:** İşlem sayısı işlem durumlarına göre nasıl dağılıyor?

**Result:** Successful (1.090), Failed (62), Cancelled (48).

**Insight:** İşlemlerin çok büyük bir kısmı (%90+) başarılıyla tamamlanmıştır. Başarısız ve iptal edilen işlemlerin oranı düşük olsa da, bu hata ve iptal kaynaklarının ayrıca incelenmesi platform güvenilirliği açısından önemlidir.

---

## Question 4

**Business Question:** Başarılı işlemlerde hangi ödeme yöntemi en yüksek işlem hacmini oluşturuyor?

**Result:** Credit Card hem işlem adedinde hem de hacimde ilk sıradadır; Bank Transfer son sırada yer alır.

**Insight:** Kredi kartı, kullanıcıların ödeme alışkanlıklarında ve yüksek tutarlı alışverişlerinde en çok tercih ettiği güvendiği kanaldır. Banka havalesinin son sırada olması, kullanıcıların anlık ve dijital ödeme yöntemlerini daha çok tercih ettiğini gösterir.

---

## Question 5

**Business Question:** Hangi müşteri segmenti en yüksek ortalama işlem tutarına sahip?

**Result:** Premium segment ortalama tutarda liderken, Standard segment toplam işlem adedinde zirvededir.

**Insight:** Premium segment yüksek ortalama tutara sahipken işlem adeti azdır; Standard segment ise yüksek hacimli ancak daha mütevazı sepet ortalamasına sahiptir. İşlem sayısı ile ortalama tutarın farklı dinamikler barındırması, segment bazlı pazarlama stratejilerinin önemini gösterir.

---

## Question 6

**Business Question:** Başarısız işlemlerde en sık görülen hata nedeni nedir?

**Result:** En yaygın hata "Insufficient Funds" (Yetersiz Bakiye) olarak öne çıkmıştır.

**Insight:** Yetersiz bakiye, kullanıcı kaynaklı en büyük başarısızlık nedenidir. Bu sorunu azaltmak için kullanıcılara işlem öncesi bakiye hatırlatmaları yapılabilir veya alternatif ödeme yöntemlerine yönlendirme sağlanabilir.

---

## Question 7

**Business Question:** Başarılı işlemlerde hangi şehir en yüksek işlem hacmini oluşturuyor?

**Result:** İstanbul hem işlem adedinde hem de hacimde ilk sıradadır, onu Ankara ve İzmir izlemektedir.

**Insight:** İstanbul'un liderliği doğrudan "en iyi performans" olarak yorumlanamaz; şehirlerin genel müşteri tabanı ve pazar büyüklüğü potansiyeli hesaba katılmalıdır. Ayrıca sistemde şehri hiç kaydedilmeyen 5 işlemin olması, veri toplama süreçlerinde iyileştirme yapılmasına işaret eder.

---

## Question 8

**Business Question:** En yüksek tutarlı 10 işlem hangileridir?

**Result:** En yüksek tutarlı ilk 10 işlemin tamamı Successful statüdedir ve çoğunluğu Travel kategorisindedir.

**Insight:** En yüksek tutarlı işlemlerin tamamının başarılı olması, yüksek limitli ödemelerde de sistem altyapısının sorunsuz çalıştığını doğrular. Ayrıca bu harcamaların farklı ödeme yöntemlerine dağılması, kullanıcıların yüksek bütçeli işlemlerde tek bir araca bağlı kalmadığını gösterir.

---

## 1. Bonus Business Question

**Business Question:** Başarılı işlemlerde iş yeri kategorilerinin işlem sayısı ve hacmi nasıl karşılaştırılıyor?

**Result:** Travel ve Electronics hacimde liderken; Grocery ve Dining işlem adetlerinde öndedir.

**Insight:** Travel ve Electronics, düşük işlem adetlerine rağmen yüksek sepet tutarlarıyla cironun ana taşıyıcılarıdır. Grocery ve Dining ise yüksek frekanslı, düşük tutarlı alışkanlıklar barındırarak platformun kullanıcı canlılığını (`retention`) destekler.

---

## 2. Bonus Business Question

**Business Question:** Tutarı 1.000’den yüksek işlemler arasında en yüksek tutarlı beş işlem hangileridir?

**Result:** 1.000 üzerindeki en yüksek 5 işlemin tamamı 25.000 tutarındadır ve Travel kategorisindedir.

**Insight:** Bu durum, sistemde tek seferde yapılabilecek maksimum işlem limitini (tavan sınır) veya seyahat harcamalarındaki standart üst paket fiyatlandırmasını doğrular. Yüksek bütçeli harcamaların seyahat odaklı olması sektörel yoğunlaşmayı net bir şekilde ortaya koymaktadır.