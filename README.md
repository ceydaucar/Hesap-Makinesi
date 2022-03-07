# Hesap Makinesi
Patika.dev > Java101 > Pratik1 - Hesap Makinesi

## Videodaki hesap makinesini switch-case kullanarak yapınız.

		import java.util.*;
		
		public class hesapMakinesi {

			public static void main(String[] args) {
				
				// Yeni bir tarayıcı(scanner) oluştur.
				Scanner sc = new Scanner(System.in);
		
				// Kullanıcıdan iki sayıyı alın.
				System.out.println("İlk sayıyı girin: ");
				int n1 = sc.nextInt();
		
				System.out.println("İkinci sayıyı girin: ");
				int n2 = sc.nextInt();
		
				// Yapılmak istenen işlemi seçin.
				System.out.println("1-Toplama\n2-Çıkarma\n3-Çarpma\n4-Bölme");
		
				System.out.print("Seçiminiz: ");
				int secim = sc.nextInt();
		
				// Seçime göre hesaplama yapın.
				switch(secim) {
				case 1:
					System.out.println("Toplam: " + (n1 + n2));
					break;
				case 2: 
					System.out.println("Çıkarma: " + (n1 - n2));
					break;
				case 3: 
					System.out.println("Çarpma: " + (n1 * n2));
					break;
				case 4:
					System.out.println("Bölme: " + (n1 / n2));
					break;
				default:
					System.out.println("Yanlış seçim yaptınız. Tekrar deneyiniz.");
	    			}
			}	
		}
