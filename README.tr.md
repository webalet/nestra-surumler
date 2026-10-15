<p align="center"><img src="ekran/logo.svg" alt="Nestra nesting programı logosu" width="420"></p>
<p align="center"><a href="README.md"><img src="ekran/flag-en.svg" height="18" alt=""> English</a> &nbsp;·&nbsp; <a href="README.tr.md"><img src="ekran/flag-tr.svg" height="18" alt=""> <b>Türkçe</b></a></p>

# Nestra: lazer, plazma ve CNC sac kesim için nesting (sac dizme) programı

Nestra, sac kesim için Windows'ta çalışan bir nesting programıdır. Parçaları saca en az fire kalacak şekilde dizer, sacı sıkıştırır ve kesim makineniz için dosyaları yazar. Kurduğunuz bilgisayarda kendi başına çalışır: hesap yok, bulut yok, çalışmak için internet gerekmez.

**Program Türkçedir.** Türkçe Windows'ta kendiliğinden Türkçe açılır, istenirse Ayarlar'dan İngilizceye geçilir. Bu sayfadaki resimler İngilizce arayüzden alınmıştır, Türkçede aynı ekranlar Türkçe görünür.

Program çalışan bir lazer kesim atölyesinin içinde yazıldı ve gerçek üretim işleriyle ayarlandı: birkaç büyük parçadan, binlerce küçük parçalı plakalara kadar.

[**Son sürümü indir**](https://nestracam.com/indir/) · Windows 10 / 11, 64 bit · 14 gün ücretsiz deneme

Yeni sürümler, yardım ve lisans: **[nestracam.com](https://nestracam.com/)**. Bu sayfa artık güncellenmiyor.

![Nestra nesting programı: 3000 x 1500 saca %80,5 verimle dizilmiş 580 parça](ekran/01-nesting.png)

*Örnek iş: dokuz türden 606 parça, 3000 x 1500 sac. Motor 60 saniyede ilk saca 580 parça dizdi, sac verimi %80,5; kalanlar ikinci saca geçti. Küçük parçalar büyüklerin arasındaki boşluklara ve içlerindeki deliklere yerleşti.*

## Kimler için

- Her gün sac dizen lazer, plazma ve su jeti kesim atölyeleri
- Kesim programını hazırlayan, işlerde fireyi azaltmak isteyen çizimciler
- Kendi parçasını kesen, basit ve internetsiz bir nesting programı arayan üreticiler

## Dizilim motoru

Programın en çok emek verdiğimiz kısmı.

**Gerçek şekle göre dizme.** Parçalar dış kutularına göre değil, gerçek dış hatlarına göre dizilir. En sıkı duruşu bulmak için serbestçe döndürülür.

**Binlerce deneme, en iyisi kalır.** Motor bilgisayarın bütün çekirdeklerine dağılıp aynı anda çok sayıda farklı dizilim dener. Ekranda hep o ana kadarki en iyi dizilim durur, sonuç hiçbir zaman kötüleşmez. Ne kadar çalışacağını siz yazarsınız; istediğiniz an Sonlandır'a basarsınız, ekrandaki sonuç kalır.

**Sac sıkıştırma.** Parçalar eklendikçe bütün dizilim tekrar tekrar sıkıştırılır. Kullanılan sac boyu kısalır, kalan fire parçası büyür.

**Küçük parçalar delikleri doldurur.** Büyük parçaların arasındaki boşluklara ve içlerindeki deliklere küçük parçalar yerleşir. Bir deliğin boş kalması gerekiyorsa o parçada işaretlersiniz.

**Çok adetli parçalar düzenli dizilir.** Adedi çok olan parçalar sıra sıra, blok halinde, petek düzeninde ya da birbirine geçen çiftler olarak dizilir. Operatör plakaya bakınca neyin nerede olduğunu anlar.

**Ortak kesim.** Seçtiğiniz parçalar kenar paylaşır, tek çizgiyle kesilir.

**Elle yaptığınız korunur.** Elle koyduğunuz parçalar yerinde kalır, motor kalanı çevresine dizer. "Bu plakayı doldur" yalnız ekrandaki sacın boş kısmını doldurur.

**Çakışma yok.** Her sonuç gösterilmeden önce denetlenir. Parçaları üst üste binen ya da payı bozan bir dizilim size sunulmaz.

**Daha az sac.** Çok saclı işlerde motor son sacı boşaltmaya çalışır; mümkünse iş bir sac eksik çıkar.

## En az fire bırakan sac boyunu seçer

![Sac boyu seçimi: üç boy karşılaştırılır, en az hurda bırakan önerilir](ekran/07-sheet-size.png)

Elinizdeki sac boylarını işaretleyip Otomatik yerleştir'e basarsınız. Nestra her boyu dener, kazananı sıkıştırır, sonra her plakayı sığdığı en küçük saca geçirir. Tabloda bütün boylar yan yana görünür, en az hurda bırakan önerilir. Son sacın boş kalan ucu hurda sayılmaz: fire çizgisinden kesilip stoğa döner.

Bir işteki her sacın ölçüsü ayrı olabilir, her biri kendi dosyalarıyla çıkar.

## Takım dizme

![Takım dizme: dört farklı parçadan oluşan tam takımlar tek sacta](ekran/06-kits.png)

Parçalar takım halinde kesiliyorsa (örneğin 1 kapak + 2 braket + 2 kare + 4 tırnak) takımı tanımlar, kaç takım gerektiğini yazarsınız. Nestra yalnız tam takımları dizer: yarım takım yok, artan parça yok. Sac dolunca kalan takımlar için aynı sac tekrarlanır.

## Fire ve artık sac

- **Fire çizgisi:** son parçadan sonra kesim çizgisi eklenir, sacın kullanılmayan ucu düzgün bir fire olarak ayrılır. Taşınabilir, silinebilir ya da parçaları izleyen basamaklı (dinamik) fireye çevrilebilir.
- **Fireye göre kısalt:** sacı tek tıkla kullanılan boya küçültür ya da parçaların etrafına sarar.
- **Artık sacı plaka olarak kullanma:** "Sac ekle" ile DXF ya da DFT dosyasındaki düzensiz bir fire sacı açar, üzerine yeni parça dizersiniz.
- **Saca çizim:** sacın üzerine kendi kesim, markalama ya da boş bırakılacak alan çizgilerinizi eklersiniz.

## Kesim sırası ve simülasyon

![Kesim sekmesi: sac boyunca kesim sırası](ekran/03-cutting.png)

Kesim sırasını Nestra verir: sac başlangıç köşesinden şeritler halinde kesilir, her parçada önce delikler, en son dış hat kesilir. Dalışlar kendiliğinden uygun bir köşeye konur. Bir çizgiye tıklayıp dalışı taşıyabilir ya da boyunu değiştirebilirsiniz; tek değişiklik sactaki aynı parçanın hepsine uygulanır.

![Kesim simülasyonu](ekran/04-simulation.png)

Simülasyon kesimi ekranda oynatır; sac makineye girmeden sırayı kontrol edersiniz.

## Parça girer, kesim dosyası çıkar

![Parçalar penceresi: her parça için adet, kalınlık ve malzeme](ekran/02-parts.png)

**Giriş:** LXD, DFT ve DXF parça dosyaları. Parçalar penceresine bırakırsınız; dosya adında adet ve kalınlık yazıyorsa okunur, eksikleri siz doldurursunuz.

![Çıktı üret penceresi](ekran/05-output.png)

**Çıktı:** her dizilim için bir LXD dosyası ve bir DOC sac raporu, isterseniz DXF. Raporda sacın resmi, malzeme, verim ve kesim süresi tahmini olur. Aynı saclar adediyle birlikte bir kez yazılır. Çıktı doğrudan kesim makinesinin okuduğu klasöre gidebilir.

## Başka neler var

- Türkçe ve İngilizce arayüz. Windows'un diline göre açılır, Ayarlar'dan değişir.
- Aynı anda birden fazla iş, sekmelerde.
- `.nestra` iş dosyası; kaydetmeden kapanırsa kendiliğinden alınan kurtarma kopyası.
- Bütün sabit ayarlar tek Ayarlar penceresinde, başka bilgisayara taşımak için dışa / içe aktarma.
- Motorun işlemcinin ne kadarını kullanacağını siz seçersiniz.
- "Destek paketi oluştur": işi, günlükleri ve PC bilgisini bir zip yapar. İçine ne gireceğini görürsünüz, hiçbir yere kendiliğinden gönderilmez.

## İndirme ve kurulum

1. [nestracam.com/indir](https://nestracam.com/indir/) adresinden `Nestra-Kurulum-<sürüm>.exe` dosyasını indirin (yaklaşık 100 MB).
2. Çalıştırın. Program kullanıcı hesabınıza kurulur.

**Kurulum dosyası henüz dijital imzalı değil.** Windows ve bazı tarayıcılar yeni yayıncıların imzasız programları için uyarı verir. Dosya güvenlidir; karşılaşabileceğiniz uyarılar:

- **İndirirken:** tarayıcı dosyanın "yaygın olarak indirilmediğini" ya da "cihazınıza zarar verebileceğini" söyleyebilir. İndirilenler listesini açın, dosyanın menüsünden **Sakla / Koru** seçin (Edge ve Chrome'da yazı biraz farklıdır).
- **Kurulumu açarken:** mavi bir pencerede "Windows kişisel bilgisayarınızı korudu" yazar. **Ek bilgi**'ye, sonra **Yine de çalıştır**'a basın.
- **Antivirüs:** bazı antivirüs programları daha önce görmedikleri imzasız dosyaları engeller ya da karantinaya alır. Kurulum dosyası kaybolduysa ya da açılmıyorsa karantinadan geri alın veya istisna ekleyin.
- **Güncelleme:** güncelleme aynı sebeple takılırsa Nestra bir dakika sonra hata ve **Elle indir** düğmesi gösterir; yeni sürümü eskisinin üstüne kurarsınız.

Kurulumda LXD, DFT ve DXF dosyalarının çift tıklayınca Nestra'da açılması istenip istenmediği sorulur. İşaretlemezseniz bu dosyalar şimdi hangi programda açılıyorsa orada açılmaya devam eder.

## Deneme ve lisans

İlk açılışta "14 gün dene"ye basarsanız program anahtarsız 14 gün tam çalışır. Süre bitince kilitlenir ve anahtar ister. Açık bıraktığınız pencere de birkaç dakika içinde kilitlenir; işiniz kaybolmaz, anahtarı girince kaldığınız yerden devam edersiniz.

Lisans almak için sales@nestracam.com adresine yazın ya da WhatsApp'tan ulaşın ([nestracam.com/iletisim](https://nestracam.com/iletisim/)). Lisans kodlarınız (`NSTR-XXXX-XXXX-XXXX`) e-postayla gelir, nestracam.com'daki Hesabım sayfasında da görünür. Etkinleştirmek için durum çubuğundaki "Deneme: ..." yazısına tıklayın, kodu lisans kutusuna yapıştırın ve **Etkinleştir**'e basın. Her kod bir bilgisayarda çalışır. İnternetsiz bilgisayarda lisans penceresindeki karekodu telefonunuzla okutun. Etkinleştikten sonra lisans internetsiz çalışır.

## Güncelleme

İnternet varsa Nestra açılışta nestracam.com'daki son sürüme bakar. Yeni sürüm varsa durum çubuğunda "Güncelle" düğmesi çıkar. Basınca indirir, bütünlüğünü ve imzamızı doğrular, programı kapatıp kurar ve yeniden açar. Kaydedilmemiş işiniz varsa önce kaydetmenizi ister. İnternetsiz bilgisayarlarda hiçbir şey olmaz; kurulum dosyasını USB ile götürüp eskisinin üstüne kurmanız yeter, ayarlarınız ve işleriniz kalır.

## Bilinen sınırlar

- DXF'te çizgi, yay, daire ve LWPOLYLINE okunur. SPLINE, ELLIPSE, blok (INSERT) ve eski tip POLYLINE şimdilik okunmaz, atlanır; parça eksik gelebilir. Dizmeden önce parça listesinde şekle bakın.
- Kesim yazılımınızın bizim LXD ve DOC dosyalarımızı açtığını ilk işte kontrol edin. Kendi dosyalarınızla denemeden canlı işe vermeyin.
- Windows 7 ve 8 desteklenmez.

## Soru ve hata bildirimi

Soru ve hata bildirimi için support@nestracam.com, lisans için sales@nestracam.com adresine yazın. Hata bildirirken mümkünse Yardım → "Destek paketi oluştur" ile aldığınız zip'i ekleyin. Hakkında penceresinde program sürümü, motor sürümü ve lisans durumu görünür.
