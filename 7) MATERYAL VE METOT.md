**MATERYAL VE METOT**

**Materyal**

**DDOS (Distributed Denial of Service:Dağıtılmış Hizmet Reddi) Saldırısı**

İnternet ve web hizmetlerinin günlük faaliyetlerimizde çok önemli bir rol oynadığı günümüzün dijital ortamında, bunların sürekli kullanılabilirliğini korumak, herhangi bir kuruluşun başarısı ve güvenilirliği için çok önemlidir. 
ncak bu çaba, geçici kesintilerden hizmetin tamamen kullanılamaz hale gelmesine kadar uzanabilen ve dünya çapındaki işletmeler için önemli riskler oluşturan dağıtılmış hizmet reddi (DDoS) saldırılarının sürekli tehdidi nedeniyle sıklıkla zorlanmaktadır. Bu tür saldırıları yakalayabilen, analiz edebilen ve azaltabilen, web hizmetlerinin kesintisiz çalışmasını sağlayan bal küpleri şeklinde güçlü bir savunma aracı vardır. Bu saldırılar kötü niyetli hackerler tarafından hedef sunucuyu, ağı veya hizmeti gelen trafik seliyle boğmak ve meşru taleplere yanıt veremez hale getirmek amacıyla düzenlenir. Bu saldırılar, hedeflenen kullanıcılara erişimi engellemek veya reddetmek için hedefin altyapısındaki sınırlı bant genişliği, yetersiz işlem gücü veya yetersiz ağ yapılandırması gibi güvenlik açıklarından yararlanır. DDoS saldırıları aşağıdakiler de dahil olmak üzere hacimsel, protokol ve uygulama katmanı saldırı türleri olarak üç kategoriye ayrılır (Url-3): 

1)Hacimsel DDOS saldırıları: Bu saldırılar hedefi büyük miktarda trafikle doldurarak mevcut tüm bant genişliğini ve kaynakları tüketir.

2)Protokol DDoS Saldırıları: Bu saldırılar TCP/IP, DNS veya HTTP gibi ağ protokollerindeki açıklardan faydalanarak sunucular ve istemciler arasındaki iletişimi bozar.

3)Uygulama Katmanı DDoS Saldırıları: Bu saldırılar, kötü niyetli istekler göndererek veya uygulama açıklarından yararlanarak web sunucuları, e-posta sunucuları veya veri tabanları gibi sunucu üzerinde çalışan belirli uygulamaları veya hizmetleri hedef almaktadır.

Yapılan çalışmada linux kaliden metasploite yapılan ddos saldırısı sonucu hem ağ trafiği takibi üzerinden hem de honeypot üzerinden analiz ve karşılaştırma incelemeleri yapılması amaçlanmıştır. 
Yapılan saldırıda ilk başta metasploite ait ait açık portları belirlemek adına nmap taraması gerçekleştirilmiştir. 

**Wireshark  ve Wireshark ile Ağ Trafiğinin İzlenmesi**

Günümüzde ağ iletişimi için en yaygın kullanılan protokol koleksiyonu, iletişimi kolaylaştırmak için dijital bilgi paketleri ve alt protokoller kullanan TCP/IP'dir.
Bu nedenle, sağlam ve güvenilir veri aktarımı için bu paketlerin ve protokollerin yapısının ve içeriğinin kapsamlı bir analizi gereklidir.
Bu, yalnızca herhangi bir ağ arayüzüne (ethernet vb.) giden ve gelen paketleri ve protokolleri incelemeyi mümkün kılan ağ paket analizinin ana işlevidir. 
Wireshark, bilgisayar ağ trafiğini kaydetmeyi ve içeriğini etkileşimli olarak incelemeyi ve gözlemlemeyi mümkün kılan bir ağ paketi ve protokol analizi programı olarak bilinen ağ paket analizi için kullanılan araçtır. 
Kullanımına göre uyarlanmış çok sayıda özelliği ile, bugün mevcut olan türünün en popüler ve pratik araçları arasındadır. 
Ağ performansıyla ilgili sorunları tanımlamada, güvenlik ihlallerini tespit etmede ve sistem değerlendirmeleri yapmada kapsamlı bilgileri eş zamanlı olarak gözlemleyerek ağ analistlerine faydalı bilgiler veren güvenilir ve verimli bir çözüm sunmaktadır. 
Filtreleme özellikleri, üretkenliği hızlandıran değerli bir özellik olan ilgili veri paketlerine odaklanmayı kolaylaştırır. 
Uzmanlar bu verileri ağ üzerinden geçen her paketi ayrıntılı olarak incelemek ve güvenlik açıklarını bulmak için kullanabilir. 

Birçok bilişim araştırmacısı ağ analizi alanına yeni girmiştir. Çeşitli ağ protokolleri (ARP, CDP, RIP, OSPF) ile ağ trafiği dinlenerek ya da gönderilen paketleri toplayabilen “protokol analizörleri” gibi programlar kullanılarak “koklanabilir”. 
Bilgisayar ağıyla ilgili suçlarda paket görüntüleyiciler ve ağ odaklı adli bilişim uzmanları (Kent vd., 2006; Url-4; Url-5; Url-6; Url-7). “tcpdump” Unix/Linux işletim sistemi için en iyi bilinen ‘sniffer’ (ağ analizi ve dinleme) programı/komutudur (MEGEP, 2008).  HTTP, HTTPS, POP (Post Office Protocol; Postane Prokolü) , SMTP (Simple Mail Transfer Protocol; Basit Posta Aktarım Protokolü ), Telnet ve SSH dahil olmak üzere çeşitli ağ trafiği türleri aracılığıyla çeşitli veriler toplanabilir. 
Ağ trafiğinden sorumlu sistem yöneticileri için e-posta mesajları ve İnternet trafiği gibi veriler çok önemlidir. Ağ üzerinden toplanan verilerdeki değişimler, analizörlerin analiz işlemi sırasında daha az hassas hale gelmesine neden olabilir.  
Bu tür durumlara örnek olarak TCP yönlendirme, “proxy” sunucuları, paket yönlendirme, web ve e-posta adları, IP (İnternet Protokolü) adresi ve e-posta adresi ele geçirme, oturum engelleme ve DNS(Domain Name System: Alan adı sistemi) sahteciliği verilebilir (Casey, 2004b; Nikkel, 2005).  
Wireshark veri paketlerini kaydeder ve paket yakalama başlatıldığında tüm ağ arayüzlerini dinler.
Bu prosedürü yalnızca seçilen arayüzden gelen trafiği analiz edecek şekilde yapılandırarak, verimsiz geniş ağ analizi azaltılabilir ve hedeflenen incelemeler için zaman ve kaynak tasarrufu sağlanabilir. 
Wireshark programı açık kaynak kodlu ve ücretsizdir. Wireshark bir Windows PC'ye yüklendiğinde, WinPcaP aracı dahil edilir. WinPcaP, Ethernet kartı aracılığıyla aktif internet bağlantısına göz kulak olmasını sağlar. Wireshark arayüzü grafiksel olarak kullanılırken, WinPcaP asıl işi gerçekleştirir.

Wireshark: PCAP (Packet Capture) ve GUI (Graphical User Interface) özelliklere sahiptir. PCAP ile ağ trafiği gözlemlenir. 

GUI ise kolaylıkla kullanılabilir arayüz vermektedir. Wireshark’ın özellikleri şunlardır(Url-4; Url-5; Url-8; Url-9):

•	Kullanımı kolay ve ücretsiz ağ izlemede Windows, Linux ve MacOS gibi çeşitli işletim sistemlerini desteklemektedir.

•	Çeşitli faktörlere dayalı paket filtreleme desteği ve yakalanan paketler çeşitli şekillerde depolanabilir.

•	Birçok şaşırtıcı yeteneği arasında parselleri hızlı bir şekilde yakalama ve gösterme yeteneği de var.

•	Ağ sorunlarını tanımlamak ve düzeltmek için sunduğu kapsamlı verileri kullanır.

•	Belirli protokollerin ağ içinde nasıl davrandığı hakkında analiz hizmetleri sunmaktadır.

•	Performans ve güvenlik değerlendirmesi ile sorunsuz çalışmayı garanti etmek için ağ performansını izler.

Böylece ağ güvenliği risklerini belirler ve değerlendirir.

•	İyi derecede grafik arayüzüne sahiptir ve paketlerin renklendirilmesi vb. ile görsel olarak kolay paket analizine olanak sağlar.

Yapılan çalışmada kaliden nmap taraması yapılarak belirlenen açık portlardan 21, 22, 23 olan portlar dikkate alınarak metasploite DDOS saldırısı telnet olan 23.porta gerçekleştirilmiştir. 

Wireshark da ilgili ıp adresi ve portlara göre filtreleme işlemi yapılarak wireshark incelemesi yapılmıştır.

**Metot**

**Tpot Honeypot’un Kurulması**

T-pot kurulumu için gereksinimler şunlardır (Url-10):

•	Yeterli bellek kapasitesi (4GB RAM) olmalı

•	Hızlı veri erişimi ve depolama için 60 GB SSD olmalı

•	Dinamik IP adresi ataması için DHCP ( Dynamic Host Configuration Protocol: Dinamik Ana Bilgisayar Yapılandırma Protokolü) ile ağ bağlantısı ve  çalışan proxy kullanılmayan bir internet (web) sayfası olmalıdır.

Kurulum için gerekenler 42 MB boyutunda bir ISO dosyasının indirilmesi gerekir. Kurulum yapılacak sunucunun internete açık durumda olması gereklidir.

T-Pot, hepsi bir arada, isteğe bağlı olarak dağıtılmış, çok kanallı (amd64, arm64) bal küpü platformudur,  20'den fazla honeypotu ve Elastik Yığın, animasyonlu canlı saldırı haritaları ve aldatma deneyimini daha da iyileştirmek için birçok güvenlik aracı kullanarak sayısız görselleştirme seçeneğini destekler (Url-10). 

Sistem gereksinimlerini karşılamak ve T-Pot kurulumu için en az 8-16 GB RAM, 128 GB boş disk alanı ve çalışan (filtrelenmemiş giden) bir internet bağlantısı gerekir(Tablo 1). 

Çalışan, desteklenen bir dağıtım indirin veya kullanın. ISO'yu mümkün olduğunca az paket / hizmet ile yükleyin (ssh gereklidir). 

**Tablo 1.** Tpot honeypot kurulum gereksinimleri (Url-10)

![gereksinim](https://github.com/user-attachments/assets/99444de4-e0d1-4ef2-b00d-df1fab839d01)


**Tablo 2.** Tpot ve ağ trafiğinde gerekli port ve protokol yönetimi (Url-10)
 
![t_pot_neypot_port ve işlevlere göre_ayrım](https://github.com/user-attachments/assets/461c76bd-b29f-48a9-a157-2188f156219a)

Kötü niyetli saldırganların bırakmış olduğu log kayıtlarına göre Tpot için ağ trafiğini izleme ve ilgili port ve protokole göre yönetimi Tablo 2 de gösterilmiştir. 

Protokole bağlı port ve yönelime göre nasıl bir tpot honeypote saldırdığı görülmektedir (Url-10).

SaaS hizmetlerinin bağlantı noktaları ve kullanılabilirliği coğrafi konumunuza göre değişebilir. 

Bazı honeypotların tam işlevselliğe ulaşması için (örneğin Cowrie veya Log4Pot) saldırganın kötü amaçlı yazılımını indirebilmeleri için giden bağlantılar da gereklidir. 
T-Pot, Debian (Stable) ağ yükleyicisine dayanmaktadır.Honeypotdaemonlarının yanı sıra diğer destek bileşenleri de yerleştirilmiştir. 
Bu, T-Pot'un aynı ağ arayüzünde birden fazla honeypot daemonunu ve aracını çalıştırmasına izin verirken, küçük bir ayak izini korur ve her bal küpünü kendi ortamında sınırlar (Çiroğlu, 2020). 
T-POT, ücretsiz olarak dağıtılmaktadır. Güncel derlenmiş kurulum dosyası “https://github.com/telekom-security/tpotce” web sitesinden debian12 iso dosyası indirilmiştir. 
İndirilmiş olan iso dosyasını sanal makineye yükleme ve kurulum işlemleri gerçekleştirilmiştir. 
Ancak debian12 iso dosyasında ssh ayarlamalarında sorun yaşandığından dolayı Ubuntu ıso dosyası ile kurulumda gerekli ssh ayarlamaları ile cockpit ve web erişim sistemlerine erişilmiştir (Url-10). 

![ubuntu_ıso_dosyası_yuleme_1](https://github.com/user-attachments/assets/ecde9101-c330-4235-b09c-086c1b478f3c)

**Şekil 4.** Ubuntu ıso dosyasının sanal makineye yüklenmesi işlemi

![ubuntu_dil_ayari](https://github.com/user-attachments/assets/59a07bdd-c4db-43b4-aff9-4388255c03c4)

**Şekil 5.** Ubuntu dil ve klavye ayarlaması

Ubuntu dil ve klavye ayarlaması Şekil 5 de gösterilmektedir.

![ubuntu_serve_dyasi_proxysiz_yukleme](https://github.com/user-attachments/assets/242a4a07-a58f-4e1f-bf72-1734312d682b)

**Şekil 6.** Ubuntu serverin proxysiz  yüklenmesi

Ubuntu server dosyasının ve proxysiz dosyanın yüklenmesi Şekil 6 da gösterilmektedir.

![ubuntu_ıso_dosyası_yukleme_son_islem](https://github.com/user-attachments/assets/9baa9ed9-0f41-4791-8708-9fa5410d4e41)

**Şekil 7.** Ubuntu ıso dosyasının son işlemi

Ubuntu ıso dosyasının sanal makine yüklemek için gerekli son işlemler Şekil 7 de gösterilmektedir.

![T_pot_installer_kurulumu](https://github.com/user-attachments/assets/861f525c-883a-4c5f-8c51-24f3e1d1bb17)

**Şekil 8.** Tpot installer(kurulumu)

Sanal makineye Ubuntu server ıso dosyası kurulumu ve gerekli işlemlerin yapılmasından sonra tpot kurulumu işlemlerine geçilmiştir. 
Tpot kurulumu için ilk başta “ git clone https://github.com/telekom-security/tpotce.git ” ile ilgili Tpot kurulum işlemlerinin işlemi gerçekleşmiş oldu (Url-10) (Şekil 8).

![T_pot_isntaller_işlemeinde_yukleme_goruntusu](https://github.com/user-attachments/assets/b4606a5e-fe61-4271-a5a7-94f6ea970239)

**Şekil 9.** Tpot installer(kurulum) işlemleri

“~/tpotce/install.sh” ile Tpot installer işlemlerine Şekil 9 da görüldüğü gibi installe y (yes) denilenerek Tpot kurulumuna başlanmış oldu.

![Tpot_installer yüklemesi](https://github.com/user-attachments/assets/962e7e2d-637e-4d20-8152-ed1349de85e4)
**Şekil 10.** Tpot tipi seçimi

Tpot kurulumu sonrasında tpot tipi seçimi için (H)ive, (S)ensor, (M)obile gibi üç farklı Tpot tipine göre hive olarak seçim gerçekleştirildi (Şekil 10).

![T_pot_honeypotlar_yuklenenler](https://github.com/user-attachments/assets/4cfbc246-03a3-4825-b0bb-028c5833a7a3)

**Şekil 11.** Yüklenen honeypotlar

Kurulan Tpot ile yüklenen honeypotlar Şekil 11 de görülmektedir.

![T_pot_honeypot](https://github.com/user-attachments/assets/7ba3aa83-f875-413d-9819-0c8b13ffcbd9)

**Şekil 12.** Tpot  yüklenme ekranı

Yapılan tüm işlemler soncu ilgili ssh ayarlamaları ve yeniden başlatma ile ilgili ssh ayarlama işlemleri öncesi kurulum Şekil 12 de görülmektedir. Tüm bu ayarlamalar soncu web adresine ulaşmak için Tpot’un  ip adresini doğru öğrenebilmek için ip a ile ilgili ip adresi öğrenilmiştir.
Debian 12 ile tpot kurulumunda ssh ayarlamalarında sorun yaşandığından dolayı Ubuntu ıso dosyası ile tpot kurulumu ile hem web adresi https://IP adresi:64293 ile Ubuntu ekranına oradan da gerekli ayarlamalar ile https://IP adresi:64297 cockpit adresi (Kibana-Tpot)ekranına ulaşılmıştır.

![Ubuntu server ile yüklenen Tpot sanal makinesi](https://github.com/user-attachments/assets/7407f595-ea19-4a81-b8db-5acb33f799be)

**Şekil 13.** Ubuntu serverdeki ile Tpot sanal makinesi

Vmwarede tüm Tpot kurulumu sonrasında sanal makine içindeki Tpot sanal makinesinin ekranı Şekil 13 de görülmektedir.

![Tpot honeypot-ubuntu server ekranı](https://github.com/user-attachments/assets/4dc45899-1a31-4d39-8370-5e4ad1bcb768)

**Şekil 14.** Tpot honeypot-ubuntu server ekranı

Tpot sanal makinesi açıldığında ubuntunun server ekranı Şekil 14 de görülmektedir.

Tpot honeypota ait ip adresini öğrenmek için ip a veya ifconfig yazarak ens 33 de yer alan ip adresi öğrenilmektedir.

![T_potun serverdeki çalışma durumu](https://github.com/user-attachments/assets/98f52ac6-47e4-46d5-ba48-fd5f2029ee78)
**Şekil 15.** T_potun serverdeki çalışma durumu

Ubuntu serverde tpotu başlatmak için sudo systemctl start tpot denilerek sistem başlatılır. 
Sistemin çalışır olup olmadığını sudo systemctl status tpot denilerek sorgulanmaktadır (Şekil 15).

![weberisimsistemi](https://github.com/user-attachments/assets/52f2d036-2c6a-41bb-a12a-8855d357376d)
**Şekil 16.** Web erişim sistemi

https://ip adresi:64293 ile web erişim (ubuntu) sistemine girilmiştir. Kullanıcı adı ve şifre ile  sisteme girilmektedir(Şekil 16).

![Web_sisteminde_yer alan_terminalden sistemin_calıstıgını gosteren_komut_ve_ciktilar](https://github.com/user-attachments/assets/bb694332-273b-4c5f-b6a2-934cdf2f708e)

**Şekil 17.** Web sisteminde yer alan terminalden sistemin çalıştığını gösteren komut ve çıktılar 

Web sisteminde yer alan terminalden sistemin çalıştığını gösteren komut ve çıktılar Şekil 17 de görülmektedir.

![T_pot_ekranına_ulasmak_icin_sisteme](https://github.com/user-attachments/assets/bdc8c2dc-c50a-4940-86a8-2c6a36de9c59)

**Şekil 18.** https://ip adresi:64297

https://ip adresi:64297 yazılarak aşağıda yer alan ip adresi sistemine ilerle (güvenli değil) basılarak  sisteme geçiş yapılır (Şekil 18 ). 

Yan taraftaki sekmeden https://ip adresi:64297 ile web erişim ekranına(kibanaya) erişme ekranına gerekli kullanıcı adı ve şifre yazılarak kibana ekranına ulaşılmaya gidilmektedir.

![T_pot_kibana_ekrani](https://github.com/user-attachments/assets/1a2c8a6e-b3ca-4adf-a942-91b650e88a77)

**Şekil 19.** Tpot kibanaya erişme ekranı

https://ip adresi:64297 ile Tpot cockpit erişim ekranına(Kİbanaya) ulaşılmıştır. Bu ekranda Attack Map, Cyberchef, Elasticvue, Kibana, Spiderfoot, SecurityMeter, T-pot Readme, T-pot @ Github bölümlerinden oluşmaktadır.

![Elastic_ekran](https://github.com/user-attachments/assets/bde62a16-2054-4104-8f8d-6a0bb0b58d7b)

**Şekil 20.** Dashboards ekranı

“Kibana” > Dashboard > “T-Pot” olarak sırasıyla tıklanıp saldırının etkisine bakılarak grafik ve sonuçlar analiz edilir(Şekil 20).
