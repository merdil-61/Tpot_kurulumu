**Tpot honeypot**

![Tpot honeypot](https://github.com/user-attachments/assets/585386f1-7174-4c7e-9246-baa15e799255)

Şekil 1.Honeypotun tarihi geçmişi (Fruhlinger, 2019).

1986'da Cliff Stoll, Lawrence Berkeley Ulusal Laboratuvarı'na Sistemler Direktörü olarak atandı. 

Bir gün, Cliff bir grup hesabın tehlikeye atıldığını fark etti ve herhangi bir hacker'ı çekmek ve onu tanımlamak için zafiyet açıklarını alan cihazlar yaratmaya karar verdi 

ve 1990 yılında tüm dünyaya Honeypot adlı yeni bir terim kazandırmıştır(Fruhlinger, 2019; Honeypot, 2020) (Şekil 1).

İlk honeypot yazılımı 1998 yılında yazılmış Cybercop Sting adındaki yazılımdır. 

Bu yazılım Decoy Server olarak da bilinmektedir. 

Decoy Server, Telnet ve SMTP ( Simple Mail Transfer Protocol: Basit Posta Aktarım Protokolü) gibi servislerini simüle edebilme özelliğine sahiptir.

Oldukça limitli bir kullanıma ve log kayıtlama yeteneğine sahip olsa da saldırgan ataklarını analiz etmede faydalı bir yazılım içermekteydi (Sharma, 2016).

T pot honeypot, adını ayıların büyük bir mutlulukla yedikleri bal kovanından almaktadır. 

Bu terim aslında bir kinaye olarak kullanılmaktadır (Zakariya ve Kiah, 2012). 

Bu sistem saldırganların diğer sistemlere saldırmalarını önlemeye yönelik açıkta bırakılan kovanı ifade etmektedir.

Özel Docker kapsayıcılarını dağıtan çok amaçlı bir Honeypot sistemidir.

T-Pot, konteyner adı verilen örneklerde sanal işletim sistemlerinde yazılım çalıştırabilen bir program olan Docker'ı kullanmaktadır (Combe, Martin ve Di Pietro, 2016; Kılınç ve Can, 2023).

Bu konteynerlar, ana makinede kolayca yönetilebilir, yapılandırılabilir ve tek bir sanal makine ile birçok Docker kapsayıcısını çalıştırabilir. 

Yani T-Pot sistemi, her kapsayıcıdan tüm logları toplar ve bunları, yöneticiye her hizmete yönelik tüm saldırıların ön uç görünümünü sağlayan elastik bir yığında merkezileştirir. 

Bu ortam kendini çeşitli zafiyetlere açık servisleri barındıran sahte bir sunucu role bürünerek yerel ağ veya dış ağa konumlandırılan hizmetlerdir.

Böylece, saldırıların daha ayrıntılı olarak analiz edilebilmesi için kötü amaçlı yazılım örnekleri de yakalanır.

Bu sistemler, kötü niyetli saldırganları tuzağa düşürmek için tasarlanmış sistemlerdir.

Saldırganların hareketlerini izleyerek onların kullandıkları yöntemleri analiz eder. 

Böylece saldırganların araçları ve teknikleri hakkında veri toplamak ve etkili savunma önlemleri oluşturmaya yardımcı olmakta kullanılmaktadır (Chauhan ve Shiwani, 2017; Livshitz, 2020; Çetin, 2024).

Honeypot'lar, özellikle de harici dağıtımlar tarafından toplanan veri miktarı, manuel olarak ayrıştırmanın artık pratik olmadığı noktayı hızla aşabilir.

Log toplama platformları canlı izleme özellikleri ve uyarılar da sağlayabilir.

Bu, veri toplamaktan ziyade saldırılara yanıt vermek amacıyla Honeypot'ları dağıtırken özellikle faydalıdır.

Cowrie honeypot, Django Honeypot, Conpot (Scada honeypot), HoneyDrive, Miniprint, HonTel, BlueHive gibi T-pot honeypot araçları vardır. 

Varsayılan olarak, Cowrie yalnızca SSH'yi açığa çıkaracaktır. 

Bu, düşmanların yalnızca SSH hizmetine saldırarak bal küpünü tehlikeye atabilecekleri anlamına gelir (Çetin, 2024; Url-1; Url-2). 

Tipik bir SSH kurulumunun sunduğu saldırı yüzeyi sınırlıdır, bu nedenle hizmete yönelik saldırıların çoğu kaba kuvvet saldırıları şeklinde olacaktır.

Bu saldırılara karşı savunma yapmak çoğu durumda nispeten basittir çünkü yalnızca açık anahtarlı kimlik doğrulamaya izin vererek veya güçlü parolalar kullanarak bu saldırılar bertaraf edilebilir. 

Bu saldırılar tamamen göz ardı edilmemelidir, çünkü o kadar çok saldırı vardır ki bir noktada saldırıya uğramanız neredeyse garantidir.

Eski Cowrie dağıtımlarına karşı kullanılan en yaygın 200 kimlik bilgisinin bir koleksiyonu demo makinesinde bırakılmıştır ve aşağıdaki soruları yanıtlamak için kullanılabilir.

Şifrelerin çoğu son derece zayıftır. 

Raspberry PI'ler ve Volumio Jukebox gibi bazı cihazlar için kullanılan varsayılan kimlik bilgileri dikkate değer girişler arasındadır.

T pot honeypot ile kazanımlar şunlardır (Fruhlinger, 2020; Arora, and CatchUpdatesHi, 2020):

1) Tehdit İstihbaratı: Gelişen tehditler hakkında içgörü kazanın ve savunma stratejilerini geliştirir.
   
2) Erken Uyarı Sistemi: Kötü niyetli faaliyetleri ve olası ihlalleri erken bir aşamada tespit eder.
   
3) Saldırganların Dikkatini Dağıtma: Dikkati kritik sistemlerden uzaklaştırarak başarılı saldırıları azaltır.
   
4) Güvenlik Açığı Tanımlama: Saldırganları yakalayarak sistem güvenlik açıklarını belirler.
   
5) Eğitim ve Beceri Geliştirme: Saldırı tekniklerini analiz edin ve kontrollü bir ortamda karşı önlemler geliştirir.
    
6) Yasal ve Adli Amaçlar: Adli analiz ve yasal işlemler için ayrıntılı bilgi toplar.
    
7) Güvenlik Farkındalığı: Tehditler hakkında farkındalığı artırın ve proaktif bir güvenlik zihniyetini teşvik eder.

   




