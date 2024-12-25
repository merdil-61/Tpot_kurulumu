**SONUC VE TARTIŞMA**

**nmap taramasi**
![nmap_scan](https://github.com/user-attachments/assets/e8418f29-556d-4f40-aa15-06cb04912b0b)
![nmap_scan_2](https://github.com/user-attachments/assets/0581ee2a-06af-49ce-9a87-178922f46203)

**Şekil .** nmap taraması

İlk başta kaliden metasploite ait nmap taraması gerçekleştirilmiştir (Şekil). nmap taraması ile açık portların  belirlenmesinden sonra  yapılan saldırıda wireshark incelemesi için filtrelemede 21(ftp), 22 (ssh) ve 23 (telnet) portlar ve ilgili metasploit ip adresi de dikkate alarak wireshark filtrelemesi yapılmıştır. Kaynağın metasploit olduğu ve açık olan portlar işaretlenmiş olup kırmızı ile işaretli olan ilgili portlara yönelik wireshark filtreleme yapılmıştır.

**DDOS Saldırısı **

![DDOS_saldirisi](https://github.com/user-attachments/assets/615a30c0-b62c-4c6e-a811-031fb331fff0)

**Şekil .** Yapılan DDOS saldırısı

Kaliden metasploitin açık olan portlardan ftp olan 23.porta DDOS saldırı gerçekleştirilmiştir (Şekil ).

**Wireshark İncelemesi**

![Wireshark_filtreleme_1](https://github.com/user-attachments/assets/37a176bc-d311-4fa7-956b-8166cea11581)
*Wireshark filtreleme incelemesi**
Wireshark ağ trafiği incelemesinde filtrelemeye göre inceleme yapabilmek için ip.addr== ilgili ip adresi (metasploitin adresi) yazılıp ve deyip incelenmesi istenen portlar köşeli parantezin içine belirtilip dışına tcp.port in {port numaraları} olarak Şekil de görülmektedir. Ağ trafiği izleme aracı olan wireshark da 71341 paketin 99,9% olarak trafik ağı incelemesi gerçekleştirilmiştir.

![Wireshark_filtreleme_2](https://github.com/user-attachments/assets/35990928-b1e6-4a9a-b09c-2ff16195d66b)
*Wireshark ağ trafiği inceleme**

Yapılan DDOS saldırısı sonrası wiresharktaki yapılan filtreleme sonucu detaylı inceleme sonucu Şekilde görülmektedir. Internet Protocol version 4 de src(source;kaynak) kalinin ip adresi dst(destiantion;son durak) ise metasploitin ip adresi olup 23 port olan telnete saldırının gerçekleştiği görülmektedir. 
Ağ trafiği izleme aracı olarak toplam kaç paketin gönderildiği ve hangi porta saldırının gerçekleştiği belirlenmektedir. 

**Tpot Honeypot İncelemesi**




*Honeypot attacks bar ve histogram grafiği**

Kaliden metasploite yapılan saldırı sonrası yapılan saldırının honeypota düşmesi sonucu saldırgan gerçek bilgiyi aldığını zannedip arkasında kendisine ait birçok kayıt bırakmaktadır. Saldırı gerçek sisteme değil honeypot sistemine ulaşıp saldırıya ait bar grafiği, histogram grafikleri ve tpotu oluşturan kaynak ip adresi sistemine saldırının gerçekleştiği Şekil  de gösterilmektedir.






*Ciscoasa tpotda saldırı histogram grafiği**

Tpot honeypot türlerinden olan Ciscoasada saldırının nasıl bir etki değişimine neden olduğuna yönelik histogram grafiği Şekilde gösterilmektedir.







*Cowrie attack, bar ve histogram grafikleri**

Bir saldırgan tarafından gerçekleştirilen kaba kuvvet saldırılarını ve kabuk etkileşimini log olarak kaydetmek için tasarlanmış orta düzeyde etkileşimli bir SSH ve Telnet honeypot olan Cowrie de yapılan saldırı sonrası  bar ve histogram grafikleri Şekilde gösterilmektedir.





*Dioneaya özel dashboard sonuç grafikleri**

Dioneaya özel dashboard sonuç grafikleri Şekilde görülmektedir.






**Honeytrap sonuç*

Saldırı sonrası Tpotun içinde yer alan honeytrap sonuç değişimleri Şekil de görülmektedir.







**NGINX sonuçları*

2002 yılında Rus yazılım mühendisi Igor Sysoev tarafından özgür ve açık kaynak olarak tasarlanmış bir web server yazılımı olan Nginx; Unix tabanlı işletim sistemlerinde çalışmaktadır. Kısıtlı olarak Windows makinelerinde desteği bulunmaktadır. Daha sonra bu yazılım tüm platformlarda kullanılabilir hale getirilen sunucu haline gelmiştir. Özellikle yüksek trafikli ve yoğun istek girişi olan web siteleri için biçilmiş sunucudur. Apache ve Lightpd ile karşılaştırıldığında daha az CPU kullanılır (Deniz, 2017; Demirşen, 2023). Yapılan saldırı sonucu tpot honeypotta nginx dashboard ekranına düşen sonuçlar Şekil de gösterilmektedir.






**Suricata sonucu*

Suricata, hem saldırı algılama sistemi hem saldırı önleme sistemi olarak işlev gören ücretsiz, açık kaynak kodlu hızlı, sağlam bir ağ tehdidi algılama motoru olan bir IDS/IPS siber güvenlik aracıdır. Bu gerçek zamanlı saldırı algılama(IDS), saldırı önleme(IPS), ağ güvenliği izleme(NSM) ve çevrimdışı pcap işleme yeteneğine sahiptir. Güçlü, kapsamlı kurallar ve imzalı dilini kullanarak ağ trafiğini inceler ve karmaşık tehditlerin tespiti için güçlü komut dosyası desteğine sahiptir(Hazar, 2020). Tpotda yer alan dashboard kısmında yer alan suricata aracında yaratmış olduğu yapılan saldırının sonuç etkisi Şekilde görülmektedir.






*Suricata alert histogramları**

Suricatada yaratılan etkiyi; kategori, port ve ülkelere göre etkileri, histogram grafikleri üzerinde Şekil de gösterilmektedir.








*Suricata attacker src ıp reputation, http sonuçları ve ülkelerin durumları**

Yapılan saldırıların etkileri suricata saldırgan kaynak ip, http ve ülkelere göre değişimleri gösteren dairesel grafikler Şekilde gösterilmektedir.









*Suricata http sonuç grafikleri ve Suricata tpota etki eden ıp, mac adresleri**

Suricata saldırgan etkisini kaynak, web kullanıcı(http)-metotu ve ip mac adreslerine yönelik değişim dairesel grafikler Şekil de gösterilmektedir.







*Suricatada ilk 10 a göre ID ve IP adresleri**
Suricatada ilk 10 a göre ID ve IP adresleri Şekilde gösterilmektedir.






*Fatt tpot sonucu**
Fatt tpot honeypotun sonucu Şekilde gösterilmektedir.







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


