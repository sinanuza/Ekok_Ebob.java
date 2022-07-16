# Ekok_Ebob.java
www.patika.dev EKOK-EBOB bulma




       import java.util.Scanner;

        public class EKOK_EBOB {
        int n1, n2;
        int ebob=1, ekok=1;
        int i=1;
        System.out.println("Lutfen birinci sayiyi giriniz;");
        Scanner input = new Scanner(System.in);
        n1 = input.nextInt();
        System.out.println("Lutfen ikinci sayiyi giriniz;");
        n2 = input.nextInt();
        System.out.println("Lutfen EBOB icin '1' i ve ya EKOK icin '2' yi secin");
        int select;
        select=input.nextInt();
        switch (select){
            case 1:
                if (n1>n2) {
                    while (i <= n1) {
                        if (n1 % i == 0 && n2 % i == 0) {
                            ebob = i;
                        }
                        i++;
                    }
                } else if (n1<n2) {
                    while (i <= n2) {
                        if (n1 % i == 0 && n2 % i == 0) {
                            ebob = i;
                        }
                        i++;
                    }
                }
                System.out.println("Gidiginiz sayilarin EBOB'u: ");
                System.out.println(ebob);
                break;
            case 2:
               while (i<=(n1*n2)){
                   if(i%n1==0 && i%n2==0){
                       ekok=i;
                   }
                   i++;
               }
               System.out.println("Gidiginiz sayilarin EKOK'u: ");
                System.out.println(ekok);
               break;
        }
    }
}
