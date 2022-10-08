# hesapmakinesi

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        int n1, n2, select;

        System.out.println("İşlem yapmak istediğiniz iki sayıyı giriniz.");
        Scanner scanner = new Scanner(System.in);

        System.out.print("Birinci Sayı: ");
        n1 = scanner.nextInt();

        System.out.print("İkinci Sayı : ");
        n2 = scanner.nextInt();

        System.out.println("1)Toplama\n2)Çıkarma\n3)Çarpma\n4)Bölme");
        System.out.print("Seçiminiz : ");
        select = scanner.nextInt();

        switch (select) {
            case 1:
                System.out.println("Toplam : " + (n1 + n2));
                break;
            case 2:
                System.out.println("Fark: " + (n1 - n2));
                break;
            case 3:
                System.out.println("Çarpım : " + (n1 * n2));
                break;
            case 4:
                if (n2 != 0) {
                    System.out.println("Bölüm : " + (n1 / n2));
                } else
                    System.out.println("HATA ! İkinci sayı sıfır olamaz.");
                break;
            default:
                System.out.println("Yanlış değer girdiniz !");
        }
    }
}
