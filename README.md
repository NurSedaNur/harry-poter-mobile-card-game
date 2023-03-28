# harry-poter-mobile-card-game
 harry-poter-mobile-card-game
1.PROEJE HAKKINDA

Bu proje ile Android uygulama ve
bulut bilişim teknolojilerinin
kullanılması amaçlanmaktadır.
Projede belirtilen süre içinde zorluk
seviyesine göre kartları doğru
eşleştirmemiz gerekmektedir.
Projeyi Android uygulama olarak
geliştirmemiz beklenmektedir.
Android uygulamasında bizden 2
ekran oluşturmamız
beklenmektedir. Hem tekli hem de
çoklu oyuncular için bir giriş
ekranı ve oyun ekranı
oluşturmamız beklenmektedir.
Giriş ekranı , oyun ilk açıldığında
ekranda açılacak sayfa giriş ekranı
olmalıdır. Kullanıcı bu ekranda,
kullanıcı adı ve şifresi ile giriş
yapabilmeli, şifre değiştirebilmeli ve
kaydolabilmelidir. Oyun ekranı ise
kullanıcı giriş yaptıktan sonra
karşısına gelecek ekran oyun
ekranı olmalıdır. Burada Tek
Oyuncu ve Çoklu Oyuncu Olarak
iki farklı seçenek bulunması
istenmektedir. Oyun ekranı ilk
açıldığında “BAŞLA” butonu
bulunmalıdır. Oyuncu BAŞLA
butonuna tıkladığında oyun ve süre
başlatılması istenmektedir. Oyun
başlatıldığında kartlar kapalı
şekilde dağıtılmalıdır. Oyundaki
kartların her birinden birer çift
bulunmaktadır. Buradaki amaç
açılan kartın diğer çiftini
bulabilmektir. Oyunda kartlar ilk
olarak rastgele dağıtılması
istenmektedir.
Oyunun farklı zorluk seviyesinde
olması istenmektedir. Bunlar 2*2 ,
4*4 ve 6*6 olmak üzere 3 farklı
zorluk seviyesinde oluşturmamız
istenmektedir.
Oyun esnasında arka planda bir
müzik çalması beklenmektedir. Bu
müzik oyun oynanırken çalmaya
devam etmelidir ve 3 durumda bu
müzik değişmelidir. 1) Kartın eşi
bulunduğunda farklı bir müzik ile
uyarı verilmelidir. 2) Oyun süresi
bittiği zaman arka fon müziği
olumsuz bir uyarı vermelidir 3)
Süre bitmeden bütün kartların eşi
bulununca arka fon müziği
kazandınız anlamında olumlu bir
uyarı vermelidir. Ayrıca oyun
müziğinin istenilen durumda
tamamen kapatılabilmesi için bir
buton eklenmelidir.
Kullanıcı bilgileri telefonda
tutulmayıp bulut üzerinden
doğrulama (log-in) yapılması
istenmektedir. Kart bilgileri de
telefonda tutulmayıp bulut üzerinde
bir veri tabanında saklanmalı ve
kullanıcının oradan erişebilmesi
istenmektedir.
Oyunu tek oyuncu ve çok oyuncu
için oluşturmamız istenmektedir.
Tek oyuncuda Kartlar oyunun
başında rastgele arka yüzleri kapalı
olacak şekilde dağıtılmalıdır.
Oyuncu bir kartın üzerine
tıkladığında kart açılmalıdır. Daha
sonra oyuncu farklı bir karta
tıklayarak kartın eşini bulmaya
çalışır. Oyun süresi 45 saniye olası
istenmektedir. Oyunda her kartın
bir puanı ve ait olduğu bir ev
bulunmaktadır. Oyun skoru her
hamle sonrasında ekranda anlık
olarak gösterilmesi istenmektedir.
Oyuncunun yaptığı doğru ve yanlış
eşleştirmelere göre skor
hesaplaması yapmamız
istenmektedir.
Çoklu oyuncuda ise kartlar oyunun
başında rastgele arka yüzleri kapalı
olacak şekilde dağıtılmalıdır. 1.
Oyuncu oyuna başlar ve bir kartı
seçer. Daha sonrasında kartın eşini
bulmaya çalışır. Eğer kartın eşini
bulursa aynı oyuncu oyuna devam
eder. Eğer kartın eşini bulamazsa
sıra rakip oyuncuya geçer. Oyun
süresi 60 saniye olmalıdır. Oyunda
her kartın bir puanı ve ait olduğu
bir ev bulunmaktadır. Her oyuncu
sırayla seçim yapar. Doğru bir
eşleştirme yapan oyuncu tekrar
oynama hakkına sahiptir. Oyun
skoru her hamle sonrasında
ekranda anlık olarak gösterilmesi
istenmektedir. Oyuncunun yaptığı
doğru ve yanlış eşleştirmelere göre
skor hesaplaması yapmamız
istenmektedir.
Bulut platformunda veri tabanı
tutulması istenmiştir.
Veritabanında kullanıcı adı, şifresi,
ID bilgisi, e-posta hesabı ve kart
bilgileri (adı, evi, puanı, kartı
resmi) bilgileri tutulması
istenmiştir. Resimlerin veri tabında
Base64 tipinde tutulması
istenmiştir.


2. BAŞLANGIÇ

Öncelikle android ve java hakkında
bilgi edindik. Android ile mobil
uygulamaların nasıl yapıldığını
öğrendik.
Bizden istenen ilk arayüz giriş
ekranıydı. Giriş ekranı oluşturduk.
Bu ekranda kullanıcının giriş
yapabilmesi için kullanıcı adı ve
şifre kısımlarını oluşturduk. Diğer
arayüzümüz için ise oyun ekranı
oluşturduk. Oyun ekranında
kullanıcı giriş yaptıktan sonra
açılıyor. Burada tek oyuncu ve
çoklu oyuncu olarak iki farklı
seçenek oluşturduk.
 Veri tabanını ve resimleri fairbase
de sakladık. Veri tabanındaki
kullanıcı adı, şifresi, ID bilgileri, eposta hesabı ve kart bilgileri
bulunuyordu. Firebase , web,
andorid , ios vb. (java, flutter ,unity
, vs.) alanlarda uygulama veya
program geliştiren yazılımcılar için
backend (arka plan) hizmeti
sağlayan bir platformdur. Firebase
; uygulama yönetimi, kullanım
takip, depolama, bildirim iletme
gibi temel işlemleri sunucu taraflı
kod yazmaya ihtiyaç duymadan
yapar .Realtime Database,
Notification, Remote Config gibi
özelliklerle birlikte her uygulama
için ayrı ayrı ulaşım imkanı sağlar.
Storage (depolama) sayesinde
sunucularımızda ya da
bilgisayarlarımızda var olan metin
, resim vb. gibi dosyaları
saklayabilir , yedekleyebilir ve
kullanıcılar bu dosyaları ulaşmak
istedikleri zaman indirebilir ya da
gerektiği zaman üzerinde
güncellemeler yaparak
yükeleyebilirler . Database ( Veri
Tabanı ) sayesinde kullanıcılara
asenkron(ayrı ayrı ) yapıda çalışan
eş (gerçek)zamanlı bir NoSql veri
tabanı hizmeti verir. Normalde
mobilde ya da web ortamında veri
tabanıyla ilgili işlemler yapabilmek
için bir veri tabanı kurmak
zorundayız yoksa elimizdeki verileri
herhangi bir yerde depolama veya
saklama imkanı kolay olmayacaktı .
Oluşturduğumuz uygulamaya göre
de veri tabanına ulaşmak için
servisler yazarız, o servisleri
sunuculara kaydederiz. Fakat
Firebase’in database hizmeti ile
çok daha rahat bir şekilde bir veri
tabanını uygulamayla birleştirip
kullanabiliriz ve yeniden database
kurmamıza ve servisler yazmamıza
gerek kalmadan database ile ilgili
olan bütün işlemlerimizi ve daha
fazlasını kolaylıkla yapmamıza
yardımcı olur .
