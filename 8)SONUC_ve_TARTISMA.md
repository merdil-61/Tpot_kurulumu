**SONUC VE TARTIŞMA**

**nmap taramasi**

![nmap_scan](https://github.com/user-attachments/assets/e8418f29-556d-4f40-aa15-06cb04912b0b)
![nmap_scan_2](https://github.com/user-attachments/assets/0581ee2a-06af-49ce-9a87-178922f46203)

**Şekil.** nmap taraması

İlk başta kaliden metasploite ait nmap taraması gerçekleştirilmiştir (Şekil). nmap taraması ile açık portların  belirlenmesinden sonra  yapılan saldırıda wireshark incelemesi için filtrelemede 21(ftp), 22 (ssh) ve 23 (telnet) portlar ve ilgili metasploit ip adresi de dikkate alarak wireshark filtrelemesi yapılmıştır. Kaynağın metasploit olduğu ve açık olan portlar işaretlenmiş olup kırmızı ile işaretli olan ilgili portlara yönelik wireshark filtreleme yapılmıştır.

**DDOS Saldırısı**

![DDOS_saldirisi](https://github.com/user-attachments/assets/615a30c0-b62c-4c6e-a811-031fb331fff0)

**Şekil.** Yapılan DDOS saldırısı

Kaliden metasploitin açık olan portlardan ftp olan 23.porta DDOS saldırı gerçekleştirilmiştir (Şekil ).

**Wireshark İncelemesi**

![Wireshark filtreleme_1](https://github.com/user-attachments/assets/b1a895bb-d601-4ba0-b2d9-1a2710ddac09)

*Wireshark filtreleme incelemesi*

Wireshark ağ trafiği incelemesinde filtrelemeye göre inceleme yapabilmek için ip.addr== ilgili ip adresi (metasploitin adresi) yazılıp ve deyip incelenmesi istenen portlar köşeli parantezin içine belirtilip dışına tcp.port in {port numaraları} olarak Şekil de görülmektedir. Ağ trafiği izleme aracı olan wireshark da 71341 paketin 99,9% olarak trafik ağı incelemesi gerçekleştirilmiştir.

![Wireshark_filtreleme_2](https://github.com/user-attachments/assets/35990928-b1e6-4a9a-b09c-2ff16195d66b)

*Wireshark ağ trafiği inceleme*

Yapılan DDOS saldırısı sonrası wiresharktaki yapılan filtreleme sonucu detaylı inceleme sonucu Şekilde görülmektedir. Internet Protocol version 4 de src(source;kaynak) kalinin ip adresi dst(destiantion;son durak) ise metasploitin ip adresi olup 23 port olan telnete saldırının gerçekleştiği görülmektedir. 
Ağ trafiği izleme aracı olarak toplam kaç paketin gönderildiği ve hangi porta saldırının gerçekleştiği belirlenmektedir. 

**Tpot Honeypot İncelemesi**

![Honeypot_attack_sonuc](https://github.com/user-attachments/assets/5ec8b514-5902-4afd-b67a-bd91cdcd2172)

*Honeypot attacks bar ve histogram grafiği*

Kaliden metasploite yapılan saldırı sonrası yapılan saldırının honeypota düşmesi sonucu saldırgan gerçek bilgiyi aldığını zannedip arkasında kendisine ait birçok kayıt bırakmaktadır. Saldırı gerçek sisteme değil honeypot sistemine ulaşıp saldırıya ait bar grafiği, histogram grafikleri ve tpotu oluşturan kaynak ip adresi sistemine saldırının gerçekleştiği Şekil  de gösterilmektedir.

![Ciscoasa tpotda saldırı histogram grafiği](https://github.com/user-attachments/assets/29f1e4c1-2213-4d05-b8ac-3155d148f222)

*Ciscoasa tpotda saldırı histogram grafiği*

Tpot honeypot türlerinden olan Ciscoasada saldırının nasıl bir etki değişimine neden olduğuna yönelik histogram grafiği Şekilde gösterilmektedir.

![Cowrie_attack, bar_ve_histogram_grafikleri](https://github.com/user-attachments/assets/c199f3e5-6d17-4646-928f-922b235a2ca9)

*Cowrie attack, bar ve histogram grafikleri**

Bir saldırgan tarafından gerçekleştirilen kaba kuvvet saldırılarını ve kabuk etkileşimini log olarak kaydetmek için tasarlanmış orta düzeyde etkileşimli bir SSH ve Telnet honeypot olan Cowrie de yapılan saldırı sonrası  bar ve histogram grafikleri Şekilde gösterilmektedir.

![Dioneaya_özel_dashboard_sonuç_grafikleri](https://github.com/user-attachments/assets/3d71c091-b386-441a-bd99-8f16ee770a64)

*Dioneaya özel dashboard sonuç grafikleri*

Dioneaya özel dashboard sonuç grafikleri Şekilde görülmektedir.

![Honeytrap_sonuc](https://github.com/user-attachments/assets/6a65f776-80e1-4c1a-86e0-8b6498fce8e3)

**Honeytrap sonuç*

Saldırı sonrası Tpotun içinde yer alan honeytrap sonuç değişimleri Şekil de görülmektedir.

![NGINX_sonuc](https://github.com/user-attachments/assets/c94412c4-1672-4819-9d65-73a462e9b140)

*NGINX sonuçları*

2002 yılında Rus yazılım mühendisi Igor Sysoev tarafından özgür ve açık kaynak olarak tasarlanmış bir web server yazılımı olan Nginx; Unix tabanlı işletim sistemlerinde çalışmaktadır. Kısıtlı olarak Windows makinelerinde desteği bulunmaktadır. Daha sonra bu yazılım tüm platformlarda kullanılabilir hale getirilen sunucu haline gelmiştir. Özellikle yüksek trafikli ve yoğun istek girişi olan web siteleri için biçilmiş sunucudur. Apache ve Lightpd ile karşılaştırıldığında daha az CPU kullanılır (Deniz, 2017; Demirşen, 2023). Yapılan saldırı sonucu tpot honeypotta nginx dashboard ekranına düşen sonuçlar Şekil de gösterilmektedir. HTTP dairesel grafikte GET ve POST şeklinde sonuçlar görülmektedir.

![suricata_sonuc](https://github.com/user-attachments/assets/50c84044-b090-4a9d-a981-f7f2349699d7)

*Suricata sonucu*

Suricata, hem saldırı algılama sistemi hem saldırı önleme sistemi olarak işlev gören ücretsiz, açık kaynak kodlu hızlı, sağlam bir ağ tehdidi algılama motoru olan bir IDS/IPS siber güvenlik aracıdır. Bu gerçek zamanlı saldırı algılama(IDS), saldırı önleme(IPS), ağ güvenliği izleme(NSM) ve çevrimdışı pcap işleme yeteneğine sahiptir. Güçlü, kapsamlı kurallar ve imzalı dilini kullanarak ağ trafiğini inceler ve karmaşık tehditlerin tespiti için güçlü komut dosyası desteğine sahiptir(Hazar, 2020). Tpotda yer alan dashboard kısmında yer alan suricata aracında yaratmış olduğu yapılan saldırının sonuç etkisi Şekilde görülmektedir.

![suricata_alert_sonuc](https://github.com/user-attachments/assets/490000ed-8fe9-4cbc-97f8-6aa49c73de20)

*Suricata alert histogramları**

Suricatada yaratılan etkiyi; kategori, port ve ülkelere göre etkileri, histogram grafikleri üzerinde Şekil de gösterilmektedir.

![suricata_http_src_ip_country_results](https://github.com/user-attachments/assets/00583cea-aa4a-4135-bd19-9dbb3b215333)

*Suricata attacker src ıp reputation, http sonuçları ve ülkelerin durumları**

Yapılan saldırıların etkileri suricata saldırgan kaynak ip, http ve ülkelere göre değişimleri gösteren dairesel grafikler Şekilde gösterilmektedir.

![suricata_ip_mac_http_sonuclari](https://github.com/user-attachments/assets/9a11efff-67d0-4a35-a18a-a208f76eeb0a)

*Suricata http sonuç grafikleri ve Suricata tpota etki eden ıp, mac adresleri**

Suricata saldırgan etkisini kaynak, web kullanıcı(http)-metotu ve ip mac adreslerine yönelik değişim dairesel grafikler Şekil de gösterilmektedir.

![suricata_ID_IPve_AS_sonuclari](https://github.com/user-attachments/assets/fd5866d7-d2e7-45dc-af63-1b44c6429016)

*Suricatada ilk 10 a göre ID ve IP adresleri**
Suricatada ilk 10 a göre ID ve IP adresleri Şekilde gösterilmektedir.

![fatt_tpot_sonuc](https://github.com/user-attachments/assets/6f76d352-6f02-4490-aa3e-c4072b1e44b9)

*Fatt tpot sonucu**
Fatt tpot honeypotun sonucu Şekilde gösterilmektedir.

![fatt_tpot_ulkelere_gore_durumu](https://github.com/user-attachments/assets/cf22e218-bd80-4ad9-8c9b-19ee9eb9fa25)

*Fatt tpotun ülkelere göre durumları**
Fatt tpot honeypotun ülkelere göre durumları Şekilde gösterilmektedir.







*Fatt tpotun http ve port-ıp durumunu gösteren grafikler**
Fatt tpot honeypotun http ve port-ıp durumunu gösteren grafikler Şekilde gösterilmektedir.







*Fatt tpot honeypotun URI, AS/N ve kaynak ip adresleri**
Fatt tpot honeypotda yapılan saldırılara göre URL,AS/Nve kaynak ip adresleri Şekil de gösterilmektedir.






*Tanner tpotun saldırı sonrası durumu**
Tanner tpot honeypotta yapılan saldırı etkisi Şekilde gösterilmektedir.  





**Tanner tpotun http e göre pasta sonuç grafikleri*
Tanner tpot honeypotun http e göre pasta sonuç grafikleri Şekilde gösterilmektedir.








Tanner tpota etki eden  IP ve url adresleri
Tanner tpot honeypota etki eden IP ve url adresleri Şekilde gösterilmektedir.




**Spiderfoot**
Ağ güvenliği, ağ ile dijital dünya arasında değiş tokuş edilen verilerin kullanılabilirliğini ve bütünlüğünü korumak için tasarlanmış önlemleri ve faaliyetleri ifade eder. Bilgi güvenliği hem donanım hem de yazılım teknolojilerini kullanarak dijital verileri yetkisiz erişime, ifşaya, manipülasyona, değiştirmeye veya yok etmeye karşı korur.  Bilgi güvenliği alanında çalışan uzmanlar tarafından yapılan bir analize göre, orta ölçekli bir şirkete ayda yirmi binden fazla siber saldırı yapılıyor. Yapılan analizler sonucunda saldırıların çoğunda risk seviyesi yüksek olmasa da önemli veriler için yoğun bir tehlike olduğu ve bu saldırıların şiddetinin arttığı tespit edilmiştir.  Spider Foot Tehdit Güvenlik Haritası istihbarat otomasyon aracıdır.  Mevcut hemen hemen her veri kaynağıyla entegre olur ve veri analizi için bir dizi yöntem kullanarak bu verilerde gezinmeyi kolaylaştırır. Temiz ve sezgisel web tabanlı arayüz sağlamak için gömülü bir web sunucusuna sahiptir, ancak tamamen komut satırı üzerinden de kullanılabilen Python 3 ile yazılmıştır ve MIT( GPL) lisanslıdır (Url-11). SpiderFoot, hedefinizin keşfi için saldırgan olarak (örneğin bir kırmızı ekip tatbikatında veya sızma testinde) veya sizin veya kuruluşunuzun İnternet üzerinden neleri açığa çıkarmış olabileceği hakkında bilgi toplamak için savunmacı olarak kullanılabilir. Hayes & Cappa (2018),Osint'in kritik altyapısına yönelik potansiyel siber saldırıları önlemek amacıyla şirket için risk değerlendirmeleri yapmak için tpot honeypotun kullanılabileceğini göstermiştir. Bir SpiderFoot taramasında IP adresi, Etki alanı/alt etki alanı adı, Ana bilgisayar adı, Ağ alt ağı (CIDR) , ASN, E-posta adresi, Telefon numarası, Kullanıcı Adı, Kişinin adı, ve Bitcoin adresi hedeflenmektedir (Arul, 2022; Url-11). 








İlgili sistemde yapılan taramalarda spiderfootlarda özellikle honeypotu içeren ip adreslerinde tehdit algılaması görülmektedir. Böylece bilgilerimizi korumak adına kurumsal şirketlerde honeypot gibi sistemlerin kullanımının önemli olduğu alınan sonuçlarla ispatlanmıştır. Honeypotlar kendi sahte verileri ile saldırganı çeker ve saldırgan bu veriyi gerçek veri zanneder. Sonuçta spiderfootda tehlike durumlarına göre değerlendirmede ilgili tpot honeypot ip adresi  daha fazla etkilenir iken hedefte olan ip etkilenmediği görülmektedir. Hem saldırılan hedef hem de honeypot sistemine ait ip adresleri hedef olarak gösterilerek belli sonuçlar alınmıştır. Sonuçlara göre hedeflenen metasploite (EK-2, EK-3, EK-6)  veya iota (EK-4) ait hedef sonuçlarında spiderfoot etkisinde ilişki matrisleri sıfır olarak görülmektedir. Ancak genel sahte verileri içeren honeypot sistemine ait yapılan taramalarda spiderfoot taramasındaki ilişkiler sıfır olmamakla birlikte burda saldırgan arkasında birçok iz bırakmıştır (EK-5 ve EK-7). Hem kibana ekranında bunu görmekteyiz hemde spiderfoot taramasında bu görülmektedir. Hedefe göre yapılan saldırılarda az element var iken honeypotun içermiş olduğu sistemlerde elementler (EK-5 ve EK-7) fazladır. EK-8 de ise yapılan saldırılara yönelik kayıtların keşefidilip tutulduğu Discover—Logstash bilgilerini içeren ekran görüntüsü görülmektedir.EK -9 da ülkelerden kendi ülkene saldırı olduğu zaman hangi porta yönelik (ftp,telnet,ssh gibi) olduğunu gösteren Attack map haritası görülmektedir. Ek-10 da ise eğer bir dosya şifreli ise cyberchef kullanılabileceğine yönelik ilgili ekran görülmektedir. EK-11 de ise elasticvue anket değerlendirmesi sayfa resmi gösterilmiştir. EK-12, EK-13, E-14 ve EK-15 de Tpot honeypotta yer alan SecurityMeter ülkelere ve çeşitli port gibi önemli bilgilere göre durumlar gösterilmiştir.


