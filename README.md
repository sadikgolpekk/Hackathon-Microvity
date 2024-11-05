# "Microvity Game"

Simurg Takımı olarak, bu proje, **Gebze**'de gerçekleştirilen **NASA Apps Challenge 2024** etkinliği için **Kocaeli Üniversitesi** öğrencileri tarafından oluşturulmuştur. Bizden, astronotların ruhsal sağlığını olumlu yönde etkileyecek ve onları eğlendirecek bir oyun yapmamız, aynı zamanda mikroyerçekimi ortamını öğretmemiz istendi. NASA'nın yayınladığı makaleleri inceleyerek, mikroyerçekimi ve uzayda geçen süre zarfındaki etkiler üzerine daha derin bir anlayış geliştirdik. Biz de, uygun tasarımlar ile mikroyerçekimi ortamını öğretecek bir oyun geliştirdik.

Çeşitli gezegenleri öğretici bir şekilde tasarladık ve her gezegenin yerçekimi değerine göre bir mikroyerçekimi barı oluşturduk. Uzayda uzun süre kaldıkça bu bar artıyor ve gittiğimiz diğer gezegenlerde bu etki, karakterimizin yavaşlamasına yol açıyor. Gerçek hayatta bunun etkilerini kas kütlesinin zayıflaması olarak düşünebilirsiniz. Yani, uzayda uzun süre kaldıkça mikroyerçekiminin etkileri fiziksel sonuçlar doğurur.

Ayrıca, her gezegende ve uzayda özgün bir müzik tasarımı yaptık. Takım arkadaşımız **Çağatay Altıntopaç** bu müzikleri özgün bir şekilde oluşturdu. Bu şekilde astronotların kendilerini daha iyi hissetmelerini sağlamayı amaçladık.

Oyun, **Godot oyun motoru** (Godot Engine) kullanılarak geliştirilmiştir ve **GD-script** diliyle yazılmıştır. Oyunun klavye kontrolü **Arduino** ile yapılırken, joystick kontrolü de sağlanmıştır. Ayrıca, ivme (gyro) sensörü ile de testler yapılmıştır. Fakat gerçek hayatta, oyun formatına uygun olarak uzayda joystick ile kontrol daha verimli olacaktır. Bunun için **Arduino** ile **Python** arasında seri haberleşme sağladık ve normalde **W, A, S, D** yerine joystick'in X ve Y eksenlerini kullandık. Zıplamak için bir buton ekledik, ancak bu butonun tepki süresi çok hassas değildi.

Proje, **NASA Apps Challenge 2024** etkinliği için **Gebze**'de gerçekleştirilen bir hackathon sürecinde geliştirilmiştir. Etkinlik süresince sadece 36 saatlik bir süremiz olduğu için, formatı en uygun şekilde bu kadarını yapabildik. Projede görev alanlar:

- **[Toprak Yozgatlıoğlu]: Level design (seviye tasarımı)
- **[Burak Demir]: Oyun formatına uygun makalelerin hazırlanması
- **[Behiç Çelebi](https://github.com/behiccelebi)** ve **[Murat Biçici](https://github.com/muratbicici)**: Godot oyun motoru ve ana kodların yazılması
- **[Çağatay Altıntopaç](https://github.com/cagatayaltintopac)**: Müziklerin özgün bir şekilde oluşturulması (FL Studio kullanarak) ve gezegenlerin formatına uygun şekilde yapılması, ayrıca Arduino ile bilgisayar etkileşiminin yönetilmesi
- **[Sadık](https://github.com/sadik)**: Arduino-Python seri haberleşmesinin kurulması ve projenin düzgün bir şekilde formata uygun olarak yapılması ve yönetilmesi.

---

### **Mikroyerçekimi Nedir?**

**Mikroyerçekimi**, dünyadaki yerçekiminin çok daha zayıf olduğu, ancak tamamen yok olmadığı bir ortamı ifade eder. Uzayda ve çok yüksek irtifalarda, yerçekimi hala mevcut olmasına rağmen, bu kuvvet çok daha zayıftır. Astronotlar, uzayda **mikroyerçekimi** ortamında "ağırsızlık" hissi yaşarlar çünkü her şey, uzay istasyonu ile birlikte aynı hızda hareket eder.

**Mikroyerçekimi**, uzayda bir cisme etkileyen yerçekiminin oldukça düşük olduğu bir durumu tanımlar. Bu, astronotların ve diğer nesnelerin yerçekiminden kaynaklanan etkilerden çok daha hafif bir şekilde etkilenmesini sağlar. Ancak, mikroyerçekimi tamamen sıfır değildir, sadece daha azdır. Bu da bir astronotun, uzayda olduğu sürece yerçekiminin etkilerini çok az hissetmesi anlamına gelir.

---

### **Uzun Süre Mikroyerçekimine Maruz Kalmanın Etkileri**

Uzayda uzun süre kalan astronotlar, **mikroyerçekimi** nedeniyle vücutlarında birkaç fiziksel değişiklik yaşar. Bunlar şunlardır:

1. **Kas Kütlesi Kaybı**: Mikroyerçekimi ortamında kaslar, yerçekimine karşı çalışmak zorunda kalmaz, bu nedenle astronotların kas kütlesi zamanla azalır. Özellikle bacak ve sırt kasları, uzayda uzun süre kaldıkça zayıflar.

2. **Kemik Yoğunluğu Kaybı**: Uzayda uzun süre kaldıklarında astronotların kemik yoğunluğu azalır. Bu, **osteoporoz** riskini artırabilir, çünkü kemikler yerçekimi etkisiyle karşılaşmadığında zayıflar.

3. **Kan Dolaşımında Değişiklikler**: Mikroyerçekimi nedeniyle kanın vücutta daha homojen bir şekilde dağıldığı gözlemlenir. Bu da kalp ve damar sisteminde bazı değişikliklere yol açabilir. Ayrıca, kalp kasları da bu durumdan etkilenebilir.

4. **Denge Problemleri**: Yerçekimi olmadığı için astronotlar, hareket etmeye alışık değildir. Bu, uzaydan Dünya'ya dönüşte denge sorunlarına yol açabilir.

5. **Göz Problemleri**: Mikroyerçekimi, astronotların göz yapısında bazı değişikliklere yol açabilir. Özellikle uzun süreli görevlerde gözde şişme ve görme bozuklukları meydana gelebilir.

Bu tür etkiler, uzayda uzun süre kalan astronotlar için sağlık açısından önemli bir problem teşkil eder. Bu yüzden, astronotlar görevlerine başlamadan önce çeşitli fiziksel testlerden geçer ve uzayda kaldıkları sürede çeşitli egzersizler yaparak kas ve kemik sağlıklarını korumaya çalışırlar.

---

### **Oyunla Bağlantı**

Bizim geliştirdiğimiz **Microvity Game**, bu mikroyerçekimi etkilerini simüle eden ve astronotların uzayda karşılaştıkları zorlukları öğretici bir şekilde sunmayı amaçlayan bir oyun deneyimi sunuyor. Oyun, astronotların mikroyerçekimi ortamında ne gibi zorluklarla karşılaştıklarını daha iyi anlamalarını sağlayacak mekanikler içeriyor. 

Özellikle, **mikroyerçekimi barı** oyundaki ana dinamiklerden biri olarak, uzayda geçirilen zaman boyunca arttıkça, oyuncunun hareketleri yavaşlıyor ve kas kütlesi kaybına dair bir simülasyon ortaya çıkıyor. Astronotların zayıflayan kasları ve kemik yoğunluğu, oyunun ilerleyen bölümlerinde oyuncunun hızını etkileyerek daha zorlu görevlerle karşılaşmalarına sebep oluyor.

Ayrıca, oyun tasarımında kullanılan **gerçek mikroyerçekimi** etkileri, astronotların uzayda daha uzun süre kalmalarının potansiyel sonuçlarını deneyimlemelerini sağlıyor. Oyuncular, uzayda kalma süresine göre kas ve kemik sağlıklarını korumak için egzersiz yaparak bu olumsuz etkilerle başa çıkmaya çalışıyorlar. Bu şekilde, astronotların mikroyerçekimi ortamında karşılaştıkları fiziksel değişiklikler hakkında bilgi edinirken, eğlenceli bir deneyim yaşamalarını sağlıyoruz.

Oyunumuz, sadece eğlenceli bir deneyim sunmakla kalmayıp, astronotların uzayda karşılaştıkları sağlık problemleri konusunda farkındalık yaratmayı da amaçlamaktadır.

---

### **Demo Videosu**

Oyunumuzun demo videosunu izlemek için aşağıdaki bağlantıyı kullanabilirsiniz:

[**Microvity Game Demo**](https://youtu.be/OYuDLIv1F2k?si=i3UzsJxv6dETDeoe)
