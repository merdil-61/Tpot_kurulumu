**ÖZET**

Honeypot sistemleri, siber saldırganları yanıltmak ve saldırı yöntemlerini analiz etmek amacıyla gerçek sunucuları taklit eden sanal makine sistemleridir. 

Bu sistemler, özellikle kurumsal şirketlerdeki hassas verilerin korunmasında önemli bir rol oynar.

Honeypotlar, saldırıları gerçek sistemlere yönelmeden önce engellerken, aynı zamanda saldırı vektörlerini ve tehdit aktörlerinin stratejilerini anlamak için değerli veriler sağlar. 

Bu bağlamda, çok yönlülüğü ve kullanıcı dostu arayüzü ile öne çıkan T-Pot honeypot platformu, farklı honeypot türlerini entegre ederek kapsamlı bir siber güvenlik çözümü sunar. 

T-Pot, saldırıları görselleştirme ve analiz etme yetenekleriyle dikkat çeker.

Yapılan çalışmada, bir DDoS saldırı senaryosu üzerinden T-Pot'un işleyişi ve etkinliği incelenmiştir.

T-Pot honeypot kurulumu adım adım gerçekleştirilmiş ve saldırı senaryosu olarak bir DDoS saldırısı uygulanmıştır. 

Wireshark ile ağ trafiği analiz edilmiş, Nmap kullanılarak açık portlar tespit edilmiştir. 

Saldırganın Metasploit üzerinden gerçekleştirdiği saldırılar özellikle Telnet (23 numaralı port) üzerinden hedeflenmiştir. 

Yapılan saldırıların tümü honeypot sistemine yönlendirilmiş ve honeypot tarafından detaylı olarak kaydedilmiştir. 

Nginx, Suricata, Cowrie ve Spiderfoot gibi araçlarla log verileri analiz edilmiş; histogram ve saçılım grafikleri üzerinden sonuçlar görselleştirilmiştir.

Analiz, saldırının honeypot sistemine yönelik olduğunu açıkça ortaya koymuştur.

Bu çalışma, T-Pot honeypot sistemlerinin kurumsal ve endüstriyel şirketlerdeki veri koruma süreçlerinde etkili bir araç olduğunu göstermektedir. 

Gerçek sistemlerin güvenliğini artırmak ve tehdit aktörlerini analiz etmek için T-Pot’un entegrasyonu oldukça önemlidir. 

Bu tür sistemler, siber güvenlik stratejilerinde önemli bir yer tutarak saldırılara karşı daha proaktif bir yaklaşım sağlar.

**Anahtar Kelimeler:** DDOS, Nmap taraması, T-pot honeypot, Wireshark.
