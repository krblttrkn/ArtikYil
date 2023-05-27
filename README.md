# ÖDEV : 
## Artık Yıl Nedir?
* Java ile kullanıcının girdiği yılın artık olup olmadığını bulan programı yazınız.
* Artık yıl, Miladi takvimde 365 yerine 366 günü olan yıl. Bu fazladan gün (artık gün),normalde 28 gün olan Şubat ayına 29 Şubat'ın eklenmesi ile elde edilir. 
## Artık Yıl Nasıl Hesaplanır?
Genel bir kural olarak, artık yıllar 4 rakamının katı olan yıllardır:
* 1988, 1922, 1996, 2000, 2004, 2008, 2012, 2016, 2020, 2024 gibi.
100'ün katı olan yıllardan sadece 400'e kalansız olarak bölünebilenler artık yıldır:
* Örneğin 1200, 1600, 2000 yılları artık yıldır ancak 1700, 1800, 1900 artık yıl değildir.
Sadece 400'e tam olarak bölünebilenlerin artık yıl kabul edilmesinin nedeni, bir astronomik yılın 365,25 gün değil, yaklaşık olarak 365,242 gün olmasından kaynaklanan hatayı gidermektedir.
```
import java.util.Scanner;

public class ArtikYil {
    public static void main(String[] args) {
        int year;
        Scanner input = new Scanner(System.in);

        System.out.print("Yıl Giriniz : ");
        year = input.nextInt();

        if ((year % 4 == 0) && ((year % 100 != 0) || (year % 400 == 0))) {
            System.out.print(year + " Bir Artık Yıldır");
        }else{
            System.out.print(year + " Bir Artık Yıl Değildir.");
        }
    }
}
```
# Patika Profilim
<a href='https://academy.patika.dev/profile'><u>Patika Profilim</u></a>