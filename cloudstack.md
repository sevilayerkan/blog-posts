# Apache CloudStack’e Giriş

Merhabalar, bu yazımda CloudStack platformunun özelliklerini ve bu tarz bir teknoloji seçiminde nelere dikkat edilmesi gerektiğini kısaca incelemeye çalıştım.

---

İlk başladığında Citrix tarafından desteklenen sonrasında Citrix’in desteğini sürdürerek pek çok başarılı projeye ev sahipliği yapan Apache Foundation’a devrettiği Apache Cloudstack’i aynı OpenStack gibi çok sayıda sanal makinayı, sanal ağı, farklı hypervisorleri , farklı depolama kaynaklarını yüksek erişilebilir ve yüksek ölçeklenebilir şekilde yönetebilen açık kaynak kodlu bir bulut bilişim platformu olarak tanımlayabiliriz.

Cloudstack pek çok firma tarafından özel bulut bilişim platformu olarak kullanıldığı gibi pek çok büyük ISS tarafından müşterilerine genel bulut hizmeti veya hibrit bulut çözümleri sunmak için kulanılmakta. China Telekom, Disney, Dell, Huawei, Nokia, Sap, Zynga, CERN gibi kuruluşlar şu an hali hazırda CloudStack çözümünü kullanıyor.

CloudStack bir IaaS çözümünden beklediğimiz; işlem gücü yönetimi (compute orchestration), network as a service , kullanıcı/hesap yönetimi, güzel bir kullanıcı arabirimi ve bir API gibi pek çok özelliği tek bir çözümde birleştiren bir proje. Bu yönüyle pek çok farklı alt projeden oluşan OpenStack’den farklılaşıyor.

CloudStack yine OpenStack gibi VMware vSphere, KVM, XenServer, XenProject ve Hyper-V, bununla birlikte OVM and LXC konteynerlarını bilinen popular çoğu hypervizörü desteklemektedir.

## Case Studies — Vaka Analizleri

Karşıma çıkan bir iş için CloudStack’ı araştırdığımdan bana verilen işi, çözülmesi gereken bu sorunu daha önce birileri deneyimlemiş mi diye araştırma yaparken yerli ve yabancı bazı vaka analizi incelemelerine denk geldim ve bu konuya da biraz baktım.

Trendyol’un yaşadığı benzer bir durumu nasıl çözdüğünü inceledim. Trendyol fiziksel makinelerin cloudlaştırılması için çözümünde OpenStack, Juju, deployment tarafında Ansible, Jenkins, network analizi tarafında Skydive teknolojilerini gördüm. (İncelediğim videolara aşağıda kaynaklar kısmından ulaşabilirsiniz.)

İncelediğim bir analizde eğer bir bulut yöneticisi (orchestrator) seçiyorsak kurulum, bakım, yükseltmeyi de hesaba katmamızı, eğer bunlar seçtiğimiz teknolojiyle zor ve zaman açısından maliyetli olacaksa bu teknolojinin başından itibaren kullanılmamasını tavsiye ediyordu. Artık bir uygulamanın sadece yapabildiklerine değil ne kadar maliyetle yapabildiğine bakmam gerektiğini anlamış oldum.

---

Openstack hakkındaki yazıma: <https://medium.com/@sevilayerkan2/openstacke-giri%C5%9F-94e098bcada6> adresinden bakabilirsiniz.

---

Makalemi okuyup vakip ayırdığınız için çok teşekkür ederim :)

Eğer bir hatam olduysa, düzeltmemi istediğiniz bir yer olursa veya iletişime geçmek isterseniz Twitter ve Linkedin adreslerinden bana ulaşabilirsiniz. Twitch’teki yazılımla ilgili yayınlarım için kanalıma gelebilirsiniz. İleride yayınlayacağım yazılarda görüşmek üzere… ❤
