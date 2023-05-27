<span style="font-size: 34px;"><strong>Çok Bölgeye Yayılan Yüksek Kullanılabilirlikli Web Uygulaması</strong></span>

Bu proje, AWS'nin farklı hizmetlerini kullanarak yüksek kullanılabilirlikli bir web uygulamasını çok bölgeye dağıtmayı ve yönetmeyi amaçlamaktadır. Projede aşağıdaki özellikler ve adımlar yer almaktadır:

<span style="font-size: 34px;"><strong>Altyapı Tasarımı ve Dağıtım</strong></span>

    AWS CloudFormation veya AWS Management Console'u kullanarak çok bölgeye yayılan bir sanal özel bulut (VPC) altyapısı oluşturulmaktadır.
    Her bölge için bir Amazon EC2 örneği oluşturulmakta ve bu örnekler bir Auto Scaling grubuna eklenmektedir.
    Elastic Load Balancer (ELB) kullanılarak trafik dağıtımı yapılandırılmakta ve güvenlik duvarı (Security Group) kuralları yapılandırılmaktadır.

<span style="font-size: 34px;"><strong>Yüksek Kullanılabilirlik ve Olay Kurtarma</strong></span>

    Multi-AZ yapılandırmasına sahip Amazon RDS veritabanı örneği oluşturulmaktadır.
    S3 kullanılarak web uygulamasının statik içeriği dağıtılmaktadır.
    AWS CloudFront ile içerik dağıtım ağı (CDN) yapılandırması yapılmaktadır.
    Veri senkronizasyonu ve yedekleme için AWS Database Migration Service veya AWS Backup gibi hizmetler kullanılmaktadır.

<span style="font-size: 34px;"><strong>İzleme ve Alarm Yönetimi</strong></span>

    AWS CloudWatch hizmeti kullanılarak uygulama ve altyapı bileşenleri izlenmektedir.
    Özel CloudWatch alarmları oluşturularak önemli metrikler izlenmekte ve gerektiğinde bildirimler alınmaktadır.
    İzleme verilerini analiz etmek için AWS CloudWatch Logs ve AWS CloudWatch Insights gibi hizmetler kullanılmaktadır.

<span style="font-size: 34px;"><strong>Güvenlik ve Erişim Kontrolü</strong></span>

    IAM kullanıcıları, grupları ve rolleri oluşturularak erişim kontrolleri yapılandırılmaktadır.
    AWS Identity and Access Management (IAM) politikaları kullanılarak kaynaklara erişim sınırlanmaktadır.
    AWS WAF (Web Application Firewall) ve AWS Shield gibi hizmetlerle güvenlik önlemleri uygulanmaktadır.
