# javanotortalamasi
java ile yapılan not ortalaması projesi
import java.util.Scanner;
public class main {
    public static void main(String[] args) {
        /*
        Not Ortalaması Hesaplayan Program
Java ile Matematik, Fizik, Kimya, Türkçe, Tarih, Müzik derslerinin sınav puanlarını kullanıcıdan alan ve ortalamalarını hesaplayıp ekrana bastırılan programı yazın.
Ödev
Aynı program içerisinde koşullu ifadeler kullanılarak, eğer kullanıcının ortalaması 60'dan büyük ise ekrana "Sınıfı Geçti" , küçük ise "Sınıfta Kaldı" yazsın.
         */

            Scanner input = new Scanner(System.in);

            System.out.println("Matematik Ders Notu");
            int mat = input.nextInt();
            System.out.println("Fizik Ders Notu");
            int fiz = input.nextInt();
            System.out.println("Kimya Ders Notu");
            int kim = input.nextInt();
            System.out.println("Türkçe Ders Notu");
            int turk = input.nextInt();
            System.out.println("Tarih Ders Notu");
            int tar = input.nextInt();
            System.out.println("Müzik Ders Notu");
            int muz = input.nextInt();

            int ortalama = (mat+fiz+kim+turk+tar+muz);
            double sonuc = ortalama/6.0;
            System.out.println("Not Ortalamanız : " + sonuc);
            boolean kosul1 = 60 >= sonuc;
            boolean kosul2 = sonuc < 60;
            boolean result = !(kosul1&&kosul2) ;
            String str = result ? "Sınıfı Geçti":"Sınıfta Kaldı";
            System.out.println(str);
    }
}
