# Konversi-Nilai
package konversi.nilai;
import java.util.Scanner;
public class KonversiNilai {
  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);
    System.out.println("Konversi Nilai");
    System.out.print("Masukkan nilai kuis mahasiswa : ");
    float kuis = sc.nextInt();
    float hasilKuis = (float) (kuis * 0.2);
    System.out.print("Masukkan nilai tugas mahasiswa : ");
    float tgs = sc.nextInt();
    float hasilTgs = (float) (tgs * 0.15);
    System.out.print("Masukkan nilai ETS mahasiswa : ");
    float ets = sc.nextInt();
    float hasilEts = (float) (ets * 0.25);
    System.out.print("Masukkan nilai EAS mahasiswa : ");
    float eas = sc.nextInt();
    float hasilEas = (float) (eas * 0.4);
    float konversiNilai = (float) (hasilKuis + hasilTgs + hasilEts + hasilEas);
    System.out.println("Nilai Akhir Mahasiswa : " + konversiNilai);
    if (konversiNilai > 85 && konversiNilai <= 100) {
      System.out.println("Predikat : A/Istimewa ");
    } else if (konversiNilai >= 76 && konversiNilai <= 85) {
      System.out.println("Predikat : AB/Baik Sekali ");
    } else if (konversiNilai >= 66 && konversiNilai <= 75) {
      System.out.println("Predikat : B/Baik ");
    } else if (konversiNilai >= 61 && konversiNilai <= 65) {
      System.out.println("Predikat : BC/Cukup Baik ");
    } else if (konversiNilai >= 56 && konversiNilai <= 60) {
      System.out.println("Predikat : C/Cukup ");
    } else if (konversiNilai >= 41 && konversiNilai <= 55) {
      System.out.println("Predikat : D/Kurang ");
    } else if (konversiNilai >= 0 && konversiNilai <= 40) {
      System.out.println("Predikat : E/Kurang Sekali ");
    }
  }
}
