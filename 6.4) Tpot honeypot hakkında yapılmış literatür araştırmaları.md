**Tpot honeypot hakkında yapılmış literatür araştırmaları**

2000'li yılların başından itibaren “honeypot (bal kovanı)” terimi ilk kez akademik çalışmalarda yer almaya başlamıştır. Spitzner yaygın olarak kullanılan tpot honeypot tanımını sorgulanmak, saldırıya uğramak veya tehlikeye atılmak gibi özelliklere sahip olan bir sahte bilgisayar kaynağı tanımlamıştır. 

Tpot honeypot teknolojilerinin özel tehditlerini tespit etmek, tanımlamak ve bunlar hakkında bilgi toplamak için nasıl kullanılabileceğini tartışmışlardır (Spitzner, 2003).

Sadasivam, Samudrala ve Yang (2005) donanım gereksinimlerini sınırlamak için dağıtım için sanal makinelerin kullanılması da dahil olmak üzere üniversite kampüslerinde bal küpü sistemlerinin tasarlanması için bir çerçeve sunmaktadır.

Brown ve arkadaşları (2012) farklı saldırı paketlerini analiz etmek için farklı bulut platformlarını, Amazon EC2, Windows Azure, IBM SmartCloud'u ve honeypot'u göz önünde bulundurarak bir çalışma yürütmüşlerdir.

ABD ve Çin, ağırlıklı olarak HTTP ve SSH tabanlı Distributed Denial of Service (Dağıtılmış Hizmet Reddi-DDoS) saldırıları gerçekleştiren ülkelerdir.

Ancak bu çalışma EC2 ve Azure ile sınırlıydı. Düşük etkileşimli honeypotu esas olarak önerilen yaklaşıma odaklanmışlardır (Brown vd., 2012). 

Buvaneswari ve arkadaşları (2013). DDoS saldırılarıyla etkili bir şekilde mücadele etmek için yerel ISP (Internet Service Provider-İnternet Servis Sağlayıcı)’lere teşvik sağlayıcı olarak IHoneycol'u kullanmıştır.

Bu çerçevenin tamamı, DDoS saldırı trafiğini sırasıyla kaynağa ve hedefe yakınlaştıran Firecol-IPS (Intrusion Prevention System- Saldırı Önleme Sistemi) ve Honeypot IPS'den oluşmaktadır.

İkiz saldırı ve ölüm saldırılarının ping'i önerilen yaklaşımla etkili bir şekilde işlenmektedir. Bu protokol hafiftir ancak yüksek hesaplama yüküne sahiptir (Buavaneswari vd., 2013). 

Bir bulut ortamında, yanlış alarm oranını azaltmak için honeypot teknolojisi kullanılarak bir saldırı tespit sistemi tasarlanmıştır.

Bu teknikle, brokerların cloudlet'ler tarafından gönderilen verilere eriştiği uygulama kuralları oluşturulmuştur. Saldırı, bulut düğümlerinin her kademesinde konuşlandırılan honey ağ geçidi tarafından tespit edilir. 

Bu şemanın ana dezavantajı, her OSI katmanında uygulanmasının hızının düşmesidir (Meghani ve Sharma, 2014).

Shabtai ve arkadaşları (2016) yapmış oldukları çalışmayı iki aşamada gerçekleştirmişlerdir. İlk aşamada, gerçek yaşam veri setine oldukça benzeyen genel yöntemler kullanılarak honeytoken oluşturmuşlardır. 
İkinci aşamada, yazarlar honeytoken'ın veri tabanlarına yerleştirilmesine rağmen kullanıcı doğasının değişmediğini göstermek için çalışmayı gerçekleştirdiler (Shabtai vd., 2016).

Honeypot'lar net verileri nedeniyle güçlü bir şekilde tepki araçları sağlar. Üretim ortamlarında daha fazla veri analizi için saldırılar bulmak zordur. Genellikle veriler diğer faaliyetlerle karışır ve bu da tepki sürecini zorlaştırır.
Nawrocki ve arkadaşları (2016) honeypotları; güvenlik duvarı veya log izleme gibi diğer hedeflerden ayırmaktadır (Nawrocki vd., 2016).

Bal tuzakları ve bal ağları, ağ güvenliği ve ağ adli bilimleri alanında popüler araçlardır. Bu araçların dağıtımı ve kullanımı, dikkatlice ele alınması gereken bir dizi teknik ve yasal sorundan etkilenir. 
Sokol ve arkadaşları (2017) honeypot tuzaklarının ve honeypot ağlarının teknik yönleri açısından gizlilik sorunlarını ana hatlarıyla açıklamaktadırlar.
Araştırmacılar, gizliliğin yasal çerçevesini ve veri işlemenin yasal gerekçelerini ele almaktadırlar. Ayrıca, IP adresini de ele almaktadırlar. 
Çünkü AB yasalarına göre kişisel veri olarak kabul etmektedirler.Bu çalışmada yasal sorunların analizi AB yasalarına dayanmaktadır ve gizlilik ve ilgili konularla ilgili tartışmalarla desteklenmektedir.

Arıkan ve Benzer (2018) bir güvenlik trendi olan honeypot hakkında tanımlama yapıp dinamik bal küpü dizaynı, bal küpü sistemleri için saldırgan web uygulaması, ssh ataklarının analizi ve görselleştirilmesi gibi çalışmaları incelemişlerdir. Ayrıca Arıkan ve Benzer (2018) de Glastopf ile sql enjeksiyonu saldırısına ve yapılan saldırının kayıtlardan görüntülenmesine yönelik örnek bir uygulama gerçekleştirmişlerdir. Çalışmanın soncu olarak kullanılmayan ip adreslerine düşük etkileşimli bal küpü sistemleri kurarak saldırganın ağda yaptığı tüm hareketlerin kayıt altına alınmasını hedeflemişlerdir. 
Honeypot türleri olan Honeyd ve Sebek honeypotlar ile kayıtları merkezi sunucuda toplayarak belli zamanlarda bu kayıtları incelemiş ve yüksek risk gördüğünde durumu yöneticiye bildirmiştir. 
Bu sayede izinsiz giriş yapan saldırgan veya ağda bulunan zararlı aktiviteler kısa sürede fark edilmiştir. 
Sanal honeypotların ağdaki makinelerin karakteristik özellikleri ile aynı oranda kurulması ile sistemdeki varlıkları gizlenmiştir. 
Bu sayede saldırgana durum fark ettirilmeden gerçek ve taklit sistemler paralel olarak çalıştırılmıştır.
Tüm bu log toplama işlemlerinin ardından daha iyi analizler elde etmek adına sonuçların görselleştirilmesini MySQL de tutulan veriler ile uygun olarak çalışabilen Kippo Graph uygulamasını seçmişlerdir. 
4 ay sonunda, saldırılarda 298 ip adresi kullanılarak, SSH servisi üzerinde toplamda 23.271 adet deneme yapıldığı görülmüştür. 
IDS, IPS ve erişim denetleme listeleri gibi birçok pasif korunma yöntemleri, bilinen saldırı teknikleri üzerinde verimli bir şekilde çalışmasına karşın henüz keşfedilmemiş yöntemleri kullanan zararlı aktivitelerinin tespiti ve engellemesinde zayıf kalmaktadırlar.
Bal küpü sistemleri bu eksikliği gidererek bilinmeyen yöntemleri kullanan saldırıları yakalamayı ve üzerinde analizler yapmayı olanaklı hale getirmiştir.
İnternetin doğuşundan bu yana, web sitelerinin sayısında ve dolayısıyla bu web sitelerindeki veri miktarında katlanarak bir artış oldu.
Black hackerler, yararlı bilgiler toplamak ve ayrıca diğer kullanıcıların ihtiyaç duydukları bilgi veya hizmetlerden mahrum bırakmak için web sitelerine saldırır. 
Bu tür sorunlar ve diğer benzer saldırı türleri, tüm saldırıları kendisine alan ve gelecekte benzer saldırı türlerini tespit etmek için saldırı modellerini inceleyen "Honeypot" sistemi tarafından ele alınabilir. 
Honeypotlar, kendilerine yapılan tüm saldırılara izin verir ve saldırganların gerçek sisteme erişebildiğini düşünmelerini sağlar ve bu arada honeypotlar saldırganların tüm saldırı modellerini inceler.

Dahiya ve arkadaşları (2020) verimliliği artırmak için çeşitli honeypotlardan oluşan bir ağ oluşturdular. Honeypotlardan önce, önceden tanımlanmış bir havuz sunucusunun yardımıyla belirli bir paketin kötü amaçlı olup olmadığını tahmin eden bir filtreleme algoritması kullanmışlardır. 
Burada, havuz sunucusunun belirli veri paketlerinin göndereni hakkında herhangi bir bilgisi yoksa, İSS servis sağlayıcısının yardımı da alınmıştır. 
Daha sonra honeynet bulutunun yeteneklerini daha da artırmak için honeynet bulutlarında HTTP (Hyper-Text Transfer Protocol: Hiper-Metin Transfer Protokolü) ve FTP (File Transfer Protocol: Dosya transfer protokolü) gibi çeşitli farklı hizmet türleri dağıtılabilir.
Burada, yazarlar önerilen çalışmayı çalıştırmak için NS2(network simulator) simülatörünü kullanmışlardır ve sonuçlar, üç farklı türdeki honeypot'un verimi, bant genişliği ve hedef sunucular tarafından sağlanan tüm hizmetlerin paket kaybı gibi grafikler biçiminde alındı. 
Kötü amaçlı paketlerin tespit oranı hesaplamışlar ve honeynet bulutu tarafından sağlanan farklı hizmetler arasında karşılaştırma yapmışlardır (Dahiya vd., 2020).

Baçer ve diğerleri.2021 Secure Socket Shell ve Telnet protokollerini hedeflemek için honeypot'lar kullanır. 
Yapılan çalışma ile SSH ve Telnet honeypot verilerini incelemektedirler. Böylece, özel bir honeypot ile SSH ve Telnet hizmetlerini taklit etmeyi önermektedir.
Honeypot'lar, araştırmacıların stratejilerini inceleyebilmeleri için saldırganları cezbetmektedir ve yakalamaktadır.
Araştırmacılar saldırıları anlamak için SSH ve Telnet honeypot verilerini incelemektedirler. 
Araştırmacılar, etkili yanıtlar oluşturmak için saldırı eğilimlerini, stratejilerini ve niteliklerini anlamak için verileri değerlendirmektedirler.
SSH ve Telnet honeypot'u bu protokollere yapılan saldırıları izlemektedirler. Verileri saldırı eğilimleri ve zayıflıklar açısından analiz etmektedirler. 
Analiz sonuçları ağ güvenliğini iyileştirebilir ve etkili SSH ve Telnet savunmaları geliştirmeye yardımcı olması sağlamıştır. 
Honeypot'lar (tuzak sistemler) siber saldırı ve izinsiz giriş girişimlerini izlemek için etkili araçlardır, ancak bu tür faaliyetlerin yeterli bir miktarını yakalamak için bunlardan yeterince konuşlandırmak kolay değildir. Siber saldırılar artarken,
özellikle de kritik kurumları hedef alanlar altyapısı için daha iyi şüpheli trafik toplama yöntemleri geliştirilmelidir.

Washofsky (2021) yapmış olduğu açık kaynaklı bir honeypot yönetim çerçevesi olan T-Pot içinde bulut tabanlı bal küplerinin dağıtımını ve kullanımını araştırmaktadır.
T-Pot örnekleri, bir web sunucusu ve bir elektrik dağıtım sistemini simüle eden honeypotlar çalıştırmıştır ve ağ trafikleri önceki yerel ve bulut tabanlı bağımsız honeypot dağıtımlarıyla karşılaştırıldı. 
Sonuçlar, bulut dağıtımlarının yerel dağıtımlardan daha fazla trafik aldığını ve T-Pot kullanımının izinsiz girişleri veya saldırıları caydırmadığını göstermiştir. 
T-Pot, bulut ölçeğindeki verileri analiz etmek için güvenlik analiz araçlarını ve hizmetlerini bir araya getirerek kritik altyapı ve kurumsal kurumlar için daha sağlam siber savunma sağlamaktadır.

Kılınç ve Can (2023) bir vaka çalışması olarak bal küpleri ve türleri açıklamışlardır. Bir kurumsal işletme ağında kurulan bir Tpot hizmetinin sonuçlarını almışlardır. 
Sonuçlardan öneriler verilmiş olup çalışmanın sonuçları değerlendirilmiştir. 
Mesbah ve arkadaşları (2023) bir Scada cihazı ağındaki potansiyel kötü niyetli müdahalelerin erken tespiti ve ICS/Scada ağlarına yönelik tehditleri belirlemek için Scada bal noktalarını kullanmışlardır. 
Scada bal küplerinin analizi bize hangi protokollerin en sık saldırıya uğradığını ve saldırganların davranışlarını, konumlarını ve hedeflerini bilme olanağı sağlamaktadır. 
Bazı ICS (Identification Code Service) protokolleri ve ICS /Scada PLC (Programmable Logic Controller: Programlanabilir Mantıksal Denetleyici) 'leri ile gerçek ICS/Scada sistemlerini simüle eden Conpot adlı bir ICS/Scada honeypot kullanmışlardır.

Sethuraman ve Sudhakaran (2023) yapmış oldukları çalışma ile ilk olarak konteyner honeypotların uğraştığı kalıpları, yöntemleri ve kötü amaçlı yazılım türlerini kavrayarak, honeypot teknolojisi hakkındaki bilgi boşluklarını doldurmak için mevcut honeypot araştırmalarındaki yeni gelişmeleri incelemişlerdir. Bağımsız olarak başlatılan ve ortaklaşa yürütülen konteyner honeypot stratejileri ve çeşitli metodolojileri kapsayan geniş bir yelpazedeki çalışmalar üzerinde çalışmışlardır. 
İkinci olarak, bilimsel araştırmalara yardımcı olan çok sayıda kullanım örneğini kullanarak, tanımlama sorunları, bal küpü güvenlik sorunları ve güvenilirlik sorunları gibi konteyner bal küpleriyle ilgili bir dizi zorluğu ele almışlardır ve araştırmışlardır.
Ayrıca, kapsamlı honeypot araştırmasına dayanarak, araştırmacıların yanı sıra meraklılara tehdit istihbaratı için gerçek zamanlı akış verileri üretmede yardımcı olan konteynerli bir araştırma honeypotu olan vikrant'ı geliştirmişlerdir. 
Yapılandırılan yaklaşım izlenerek kötü niyetli kullanıcıların faaliyetleri hakkında ilgili sonuçlara varılmasını sağlayan çeşitli veri noktaları elde etmişlerdir.

Yang ve arkadaşları (2023) ağ tehdit yönetimine yönelik etkileşimli honeypot tabanlı bir yaklaşımla ilgili araştırma yapmışlardır ve sürekli saldırılara dayanırken ağ ortamı için aktif savunma önlemleri sağlayan yüksek etkileşimli bir bal küpü tehdit yönetim sistemi oluşturmak için modüler bir tasarım yaklaşımı önermişlerdir.
Modelin uygulanabilirliğini değerlendirmek için pratik testler yapılmıştır ve sistem diğer ağ tehdit yönetim sistemleri ile karşılaştırılmıştır. 
Sistem, bilgi toplama aracı olarak yüksek etkileşimli bal küpleri kullanmakta, saldırganın IP adresini sınıflandırma için birincil anahtar olarak kullanarak 1 aylık toplanan verileri biçimlendirmekte ve kullanıcı dostu bir web arayüzü sunmaktadır. 
Analiz edilen protokoller HTTP, SNMP (Simple Network Management Protocol; Basit Ağ Yönetimi İletişim Kuralı), Modbus, BACnet ve S7Comm'dur. 
Yapılan çalışma ile sistem çeşitli işletim sistemlerine uyum sağlamakta ve geleneksel ağ tehdit yönetim sistemlerine kıyasla güvenlik ve proaktivitede önemli gelişmeler göstermiştir. 
Sistemin güvenlik ve baştan çıkarma hedeflerine ulaştığını göstermekte ve honeypot teknolojisinin daha yaygın bir şekilde uygulanmasını teşvik etmektedir.

Yapılan bu proje çalışmasıyla kurulan Tpot ile bir sanal makineden diğer sanal makineye yapılan saldırı sonucunda nasıl bir etki olduğunu Tpot üzerinde yer alan honeypotlar sayesinde gözlemlemek hedeflenmiştir.
Ayrıca sistemde yer alan spiderfootda yapılacak olan tarama işlemlerinde hedef ıp adresi ve tpot honeypotun yer aldığı Ubuntu sistem ip adresi gösterilerek yapılan saldırının nasıl etkilediği gözlemlenmiştir.

Projenin çalışma planını içeren Gant Şeması şu şekildedir.

![Gant_seması](https://github.com/user-attachments/assets/f743cc4c-8f6e-45e4-9353-6053cc9ab5b0)



