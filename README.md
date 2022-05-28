# Libft

Libft [42](https://42.fr/en/homepage/) programının ana eğitim sürecinin ilk projesidir. Bu projenin amacı C dilinde yazılmış fonksiyonlardan oluşan ilk kütüphanenizi oluşturmak.

Bu projeye başlamak için bilmeniz gerekenler:
- `Makefile` nedir?
- `.c` uzantılı dosyalar
- `.h` uzantılı dosyalar
- `.a` uzantılı dosyalar

## Makefile nedir?

  Makefile temel olarak programın derleme sürecini kolaylaştırmak adına kullanılan bir dosyadır. Özellikle çok sayıda kaynak dosyasının bir arada derlendiği durumlarda sizin tanımladığınız kısayollarla, ortaya çıkartmak istediğiniz dosyayı daha hızlı şekilde oluşturmanızı sağlar. Bu proje için Makefile dosyasının bir örneğine [buradan](https://github.com/ahmettakcan/libft_rehber/blob/main/Makefile) ulaşabilirsiniz. Bu dosyada dikkat edilmesi gereken iki unsur değişkenler ve komutlardır. Örnekte bulunan `NAME = libft.a` bölümü `NAME` adında bir değişkene `libft.a` değerini atamaktadır.
  
  Değişkenleri, çağıracağımız komutları düzenlerken kullanırız. Bu değişkenler sayesinde kaynak dosyalarının isimleri gibi uzun değerler üzerinde daha hızlı işlem yapılabilir. Ayrıca kullanacağınız derleyiciyi türü gibi, kodun farklı komutlarında çağırdığınız değerleri tek bir noktadan değiştirmenizi sağlar. Örneğin, bizim durumumuzda `CC` değişkenini (yani derleyicimizi) kolaylıkla `clang` veya `gcc` olarak ayarlayabiliriz.
  
  ## Komutlar
  
  Makefile da `$(NAME)` `all` `clean` `fclean` ve `re` kurallarını içermelidir.
