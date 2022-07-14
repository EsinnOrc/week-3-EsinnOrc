# week-3-EsinnOrc

## Symfony kullanmanın avantajları
Symfony, mvc(model, views, controller) mimarisine sahip açık kaynaklı bir php frameworktür. Karmaşık web uygulamalarında tercih edilir. Hızlı ve kolay kod geliştirme yapılmasına olanak sağlamaktadır. OOP(nesne yönelimli programlama) mimarisine sahiptir. Kaynak olarak çok gelişmiştir. Yardımcı birçok uygulama yer almaktadır. Kolaylıkla kütüphane dahil edilebilir. Birden fazla kişi aynı proje de görev alabilir. Symfony oraganize bir şekilde çalışmaya olanak sağlar. Symfony sayesinde büyük oranda güvenliği düşünmemize gerek kalmaz. Bu sayede daha fazla tercih edilir.


## Symfony ile environment (ortam) ayarlama
Symfony uygulaması dev, prod ve test olmak üzere üç ortamla başlar. 
- dev: Uygulamayı yerel olarak geliştirirken kullanılır.
- prod: Uygulamayı çalıştırırken kullanılır.

Bütün ortam değişkenlerinin değerini ayaralamak için 

```ruby
php bin/console debug:dotenv
```
kullanılır.

## Yeni bir Symfony projesi oluşturmak için kullanılan composer komutu
Webapp paketi eklenmiş şekilde kurulum kodudur. 
```ruby
composer create-project symfony/skeleton:"^5.4" my_project_directory
cd my_project_directory
composer require webapp
```
Webapp paketi eklenmeden kurulum kodudur. Web uygulaması için proje geliştirilmiyorsa bu kodun kullanılması yeterlidir. 
```ruby
composer create-project symfony/skeleton:"^5.4" my_project_directory
```
Symfony CLI'yi yüklerekte yeni proje kurulumu yapılabilir. 

```ruby
scoop install symfony-cli
symfony new --webapp my_project
symfony new my_project
```

## Laravel framework ve Symfony framework arasındaki temel 2 fark
- Symfony'de veritabanı bağlantıları otamatiktir. Ancak verilen kodda belli alanların tanımlanması gerekir. Laravelde de veritabanı geçişlerini kullanır ancak alanları tanımlamaya gerek yoktur.
Symfony veritabanı için daha fazla seçenek sunmaktadır.
- laravel performansı ve hızı için tercih edilir. Symfony, karmaşık ve büyük web projelerinde tercih edilir ve büyük projeler için uygundur.
