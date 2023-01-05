import java.util.Scanner;


public class BurcProgrami {

    public static void main(String[] args){

        int month, day;

        Scanner input = new Scanner(System.in);

        System.out.println("Doğduğunuz Ayı giriniz");
        month = input.nextInt();
        System.out.println("Doğduğunuz günü giriniz");
        day = input.nextInt();



        if ( (month >=1 || month <=12) && (day >=1 || day<=31)) {
            if (month == 1){
                if (day >=1 && day <= 31){
                    if (day <= 21){
                        System.out.println("burcunuz Oğlak");
                    } else  {
                        System.out.println("Burcunuz Kova");
                    }

                }
            } else if (month == 2) {
                if (day >=1 && day <= 28){
                    if (day <= 19){
                        System.out.println("burcunuz Kova");
                    } else {
                        System.out.println("Burcunuz Balık");
                    }

                }
            } else if (month == 3) {
                if (day >=1 && day <= 31){
                    if (day <= 21){
                        System.out.println("burcunuz Balık");
                    } else {
                        System.out.println("Burcunuz Koç");
                    }

                }
            }

        } else if (month <1 || month >12){
            System.out.println("Geçersiz ay girişi");
        } else if (day <1 || day>31){
            System.out.println("Geçersiz Gün Girişi");
        }



    }


}
