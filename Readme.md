# Week5Assignment

## Aşağıdaki soruları bir cümleyle cevaplayınız. (2x10 = 20 puan)
- Soru 1: PHP PDO nedir? Hangi amaçla kullanılır?
### PDO, desteklediği veritabanları için ortak metot ve özellikleri barındıran bir OOP sınıfıdır. Veritabanı ile ilgili Php'de işlem yapabilmemizi sağlar.
örnek olarak; 
`try {
    $baglanti = new PDO("mysql:host=localhost;dbname=kisi", "root", "");
    $baglanti->setAttribute(PDO::ATTR_ERRMODE, PDO::ERRMODE_EXCEPTION);

    $kayit_sayisi = $baglanti->exec("DELETE FROM kisiler WHERE kisi_sira = 9");

    if ($kayit_sayisi > 0) {
        echo $kayit_sayisi . " kayıt silindi.";
    } else {
        echo "Herhangi bir kayıt silinemedi.";
    }

} catch (PDOException $e) {
    die($e->getMessage());
}

$baglanti = null;`

- Soru 2: DB Index nedir? Avantajları ve dezavantajları nelerdir?

## Aşağıdaki senaryoya göre symfony uygulaması oluşturunuz. (80 puan)
Symfony ile oluşturduğunuz web uygulamanızda, en az bir servisin sonucunu twig template ile ekrana çıktı olarak bastıran bir method tanımlayınız. Kullanacağınız bu servisin de başka bir servisi çağırarak kullanması gerekmektedir.

[SYMFONY PROJE LİNKİ İÇİN BURAYA TIKLAYINIZ](https://github.com/Blackcloud00/week5homework)

