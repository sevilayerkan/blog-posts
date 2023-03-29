# SDLC — Yazılım Yaşam Döngüsü

Her yazılım projesi şu üç aşamaya sahip olmalıdır: Bunlar projeye göre bazen iç içe bazen ayrıdır.

Bunlar:

- Planlama (Project management)
- Geliştirme(Source control)
- Operasyon (Build ve development)

Yani bir akış halinde gösterecek olursak yazılım geliştirmede süreç şu şekilde ilerliyor diyebiliriz basitçe: Develop -> Test -> Build -> Deploy

## DevOps

DevOps’u anlatmaya kelimeler yetmez tabi ki ama kısaca insanları, prosesleri ve teknolojileri bir araya getirerek sürekli bir değer sunmak şeklinde tanımlayabiliriz. Detaylı bilgi için bu videoya bakabilirsiniz.

<https://www.youtube.com/watch?v=0yWAtQ6wYNM>

## CI/CD

(CI-Continuous Integration yani Sürekli Entegrasyon, CD ise Continuous Delivery yani Sürekli Dağıtım)

Yazılım gelişmeye devam edecektir. Bu süreçte projede değişiklik yaptığımızda bu değişikliklerin gerekli test ve kontrollerden geçerek canlı ortama bir an önce dahil olmasını isteriz ki bu süreci CI/CD olarak adlandırıyoruz.

Örneğin projemizi konteyner üzerinde canlı ortama çıkaracağımızı varsayalım.Geliştirme aşamasından sonra,

Code -> Test -> Build Image -> Push Repo -> Deploy -> Release aşamalarından geçirmemiz gerekiyor ve bu aşamalar her bir değişiklik oldukça tekrarlanır. Adeta bir döngü gibi.

Bunlardan Kod-Test-İmaj yaratma-Repoyu Gönderme CI, Deploy ve Release(Canlıya Alma) ise CD kısmına dahilmiş gibi düşünebiliriz şimdilik. Ancak bu süreçleri birbirinin içine geçmiş bir zincir gibi düşünmek daha doğru olacaktır.

## CI/CD Süreçlerine Genel bir Bakış

Peki bu süreçlerin yönetiminde ne kullanabiliriz?

Her ihtiyaca ve yazılım geliştirme döngüsünün her bir parçasına ait bir sürü çözüm var. Her bir geliştirme adımı için ayrı teknolojiler kullanabilirsiniz. Örneğin planlama-haberleşme adımı için Jira/Slack, versiyon kontrolü-ci-build için Github, Jenkins; deployment için farklı bir araç vs. şeklinde bu böyle gidecektir. Bu yaklaşımın şöyle bir eksisi olabilir süreçler arasındaki bağlantının nasıl yapılacağı.
