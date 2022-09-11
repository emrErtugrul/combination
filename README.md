# combination


import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner inp=new Scanner(System.in);
        int n,r,i,fak=1,j,cnr,rfak=1,nr,nrfak=1,k;
        System.out.println("Lütfen N Sayısını Giriniz");
        n=inp.nextInt();

        for (i=1;i<=n;i++) {
            fak=fak*i;

        }
        System.out.println("Lütfen R Sayısın Giriniz");
        r=inp.nextInt();
        for (j=1;j<=r;j++) {
            rfak=rfak*j;

        }
        nr=n-r;
        for (k=1;k<=nr;k++) {
            nrfak=nrfak*k;

        }
        System.out.println(n+"! n Faktöriyel: "+fak);
        System.out.println(r+"! r Faktöriyel: "+rfak);
        System.out.println(nr+"! r Faktöriyel: "+nrfak);

        cnr=(fak)/(rfak*nrfak);
        System.out.println("C("+n+","+r+") Kombinasyonu: "+cnr);

    }
}
//C(n,r) = n! / (r! * (n-r)!)
