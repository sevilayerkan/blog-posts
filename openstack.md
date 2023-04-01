# Openstack’e Giriş

## OpenStack

‘King of the cloud’ yani bulutun kralı olarak adlandırılan Openstack bir ‘Cloud framework’ gibi düşünülebilir, 7 core proje birlikte tek bir çatı altında çalışabilir. Nasa ve Rackspace iş birliğinde geliştirilmeye başlanmıştır. Kimlik, storage, image, network yönetimi ve sanallaştırma yönetimi gibi çözümleri içinde barındırır. Ansible, Terraform gibi araçlarla da kullanılabilir.

Özetle; bir datacenterdaki tüm işlem, depolama, networking kaynaklarının API ve diğer authentication mekanizmaları sayesinde kontrolünü sağlayan bulut işletim sistemidir aslında. Dashboard desteği sayesinde adminlere ve kullanıcılara web interfacei aracılığı ile erişim olanağı da sağlar.

Minimum 1 node(sunucu) üzerine kurulabilir ancak önerilen node sayısı minimum 2 adettir. (Controller/Compute veya Controller/Compute + Block Storage, Object Storage node gibi) Node sayıları ihtiyaca göre değişebilir. Hybrid yapı ile public cloud firmalarına bağlanılabilir.

Kullanan bazı şirketlerden bahsedersek; Nasa, Cern, Yahoo, Deutsche Telekom, Walmart, Trendyol, MEB Fatih Projesi, Turkcell (Nesne depolama)

## Servisler

- Core (Esas) servisler : Glance (Image), Neutron (Networking), Swift (Object Storage), Keystone (Identity), Cinder (Block Storage), Nova (Compute)

- İsteğe bağlı servisler: Ironic(bare metal service), Freezer, Senlin(clustering), Throve, Manila(Shared storage service)

## MAAS: Metal As A Service

Fiziksel sunucuların sanki birer virtual makinelermiş gibi bulutta kontrol edilebilmesini sağlar. Fiziksel sunuculara erişim, kurulum ve yönetim işlemlerini gerçekleştirebiliriz.

Açık kaynak kodludur. Bu teknolojiyle uzaktan boot ederek fiziksel sunuculara Windows veya Linux OS lar kurabiliriz. Bilinen birçok OS ve ESXi ile uyum sağlar.

Ansible, Chef, Salt, Puppet gibi DevOps araçları ve diğer Openstack servisleri ile de entegrasyonu olması oldukça avantaj sağlar.

Özet olarak; MAAS bulutun hız ve esnekliğini, fiziksel (bare metal) sistemlerin gücüyle birleştirerek bize ölçeklenebilir güzel bir çözüm sunar. Adeta fiziksel makineleri clouda dönüştürür.

## Juju

Deploy, konfigure etme, scale ve operasyon işlemlerini yapmamızı sağlayan açık kaynaklı bir aplikasyon modelleme aracıdır.

Genelde MAAS ile kullanılır. OpenStack’i geniş ölçekte dağıtmayı, yapılandırmayı, ölçeklendirmeyi ve çalıştırmayı kolaylaştıran açık kaynak kodlu bir üründür.

Desteklenen herhangi bir cloud ortamında birbiriyle entegre çalışacak uygulamaların kurulumunu ve yönetimini sağlar.

Buraya kadar OpenStack, MaaS, Juju nedir, ne işe yarar buna bakmış oldum. Makalemi okuyup vakip ayırdığınız için çok teşekkür ederim. :)

---

Eğer bir hatam olduysa, düzeltmemi istediğiniz bir yer olursa veya iletişime geçmek isterseniz Twitter ve Linkedin adreslerinden bana ulaşabilirsiniz. Twitch’teki yazılımla ilgili yayınlarım için kanalıma gelebilirsiniz. İleride yayınlayacağım yazılarda görüşmek üzere… ❤
