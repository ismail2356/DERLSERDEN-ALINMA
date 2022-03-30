# DERLSERDEN-ALINMA
   // ASAL SAYI KONTROL
package asalsayıkontrol;

import java.util.Scanner;
public class AsalSayıKontrol {
    public static void main(String[] args) {
        Scanner scan= new Scanner(System.in);
        System.out.println("Lütfen bir tamsayı giriniz");
        int sayi=scan.nextInt();
        int sayac=0; // bobin tuzağı
        // tuzağımızı kurduk
        for(int i=2;i<sayi;i++){
           if( sayi%i==0){
           sayac++;
                   }
        
        }
        //tuzağı kontrol ediyoruz
        if(sayac==0)
            System.out.println(sayi + "  Sayısı asaldır");
        else{
        System.out.println(sayi + "  sayısı asal değildir ");
        }
        
    }
    
}


_________________???????????????????======================_______________==============================================
      // TAŞ KAĞIT MAKAS OYUNU

package javaapplication21;

import java.util.Scanner;
public class JavaApplication21 {

    
    public static void main(String[] args) {
        Scanner scan= new Scanner(System.in);
      System.out.println(" kağıt için 0 , makas için 1 ,taş için 2 giriniz");
      int tahmin=scan.nextInt();
      int bil=(int)(Math.random()*3);
     
      if(tahmin==bil)
          System.out.println("berabere");
      if(bil==0 && tahmin==1)
          System.out.println("bilgisiyar kağt , siz makas . siz kazandınız");
      if(bil==0 && tahmin==2)
          System.out.println("bilgisiyar kağıt siz taş . bilgisiyar kazandı");
      if(bil==1 && tahmin==0)
          System.out.println("bilgisiyar makas siz kağıt bilgisiyar kazandı ");
      if(bil==1 && tahmin==2)
          System.out.println("bilgisiyar makas siz taş  siz kazandınız");
      if(bil==2 && tahmin==0)
          System.out.println("bilgisiyar taş siz kağıt siz kazandiniz");
      if(bil==2 && tahmin==1)
          System.out.println("bilgsiyar taş siz makas bilgisiyar kazandı");
      
      
        
        
     
    }
    
}


____________________________________________________________________________________???????????????????________________________
     // DİZİNİN EN KÜÇÜK ELAMNI BULMA VE EKRANDAN DİZİ ELAMANI GİRME
     
     package dizi.en.küçük.elamanı.bulma;

import java.util.Scanner;
public class DiziEnKüçükElamanıBulma {

   
    public static void main(String[] args) {
        Scanner scan=new Scanner(System.in);
        int dizi[]= new int[4];
        System.out.println(" lütfen " + dizi.length + " kadar tamsayı giriniz");
        int i;
        for(i=0;i<dizi.length;i++){
                dizi[i]=scan.nextInt();
        System.out.println( "elmanları " +dizi[i]  + "  ");
        }
        
        int sayac=dizi[0];
        for(int j=0;j<dizi.length;j++){
            if(sayac>dizi[j]){
            sayac=dizi[j];
            
            } 
        
        }
       
        System.out.println( "en küçük eleman " +sayac);
            }
        
        
       
    
}
     
     
     ________________________)_____________________________=______________?_________________________________________-
        // ÇARPIM TABLOSU
        
        
        package carpımtablosu;


public class CarpımTablosu {

    
    public static void main(String[] args) {
        
        System.out.println("              CARPIM   TABLOSU   ");
        System.out.print("  ");
        for(int j=1;j<=9;j++)
            System.out.print("   "+j);
        
        
        System.out.println( " burası önemli" +"\n--------------------------------------");// buradaki"\n" sağında yazılanı alt satıra yazılmasını sağlar çok önenli
        for(int i=1;i<=9;i++){
            System.out.print(i + "|");
            for(int j=1;j<=9;j++){
            System.out.printf("%4d",i*j);
            
            
            }
        System.out.println();
            
            
        }
        
        
        
        
    }
    
}   



___________________=______________=_____________=________________________=________?_____________________________________________
       //  DİZİN ELAMANLAEINI KÜÇÜKTEN BÜYÜYĞE SIRLAMA
       
       
       
       package dizisıralama;


public class DiziSıralama {

    
    public static void main(String[] args) {
        int dizi[]={123,10,1,3,5,2,4,8,0,7,6};
        int gecici;
        for(int i=0;i<dizi.length;i++){
            for(int j=0;j<dizi.length-1;j++){
                if(dizi[j]>dizi[j+1]){
                    gecici=dizi[j];
                    dizi[j]=dizi[j+1];
                    dizi[j+1]=gecici;
                
                }
            
            }
        
        }
        System.out.println("elamanların sıralanması");
        for(int i =0 ; i<dizi.length;i++){
        System.out.print(dizi[i] + " ");}
        
        
        
    }
    
}   




      
      _________________________________________________________________________?________________________________________________
      // DİZİLER ÖĞRENME
      
      //diziler(arrays) En büyük avantajı döngülerde
//Dizilerin tipi istedeğimiz tipte olabilir
//dizilerde değerleri sırayla kurtucuk şeklinde bellekte yer tutar(tren vagonları gibi) 
// [] işareti genelikle bir diziyi belirtir


package dizileröğrenme;


public class DizilerÖğrenme {

    
    public static void main(String[] args) {
        int b []= new int[3];//int tipinde 3 elamanlı bir dizi tanımladım.ve sonradan değer verebilirim 
        b[2]=80;//dizinin 2. elamanına 80 değerine atadım.(int olmalı atadığım değer)
        System.out.println(b[2]);
        
        int a[]={1,2,5,6,8,7,};//6 elamanlı bir dizi ve dizilerin elamanları 0'dan başlar ve en soldan (0'dan) sağa ardışık artar
        // dizimi tanımlamama gerek yok ve dizinin elamanları bellidir
        System.out.println(a[0]);//a[0]=1, a[5]=8, a[6]=7
        
        String stri[]={"Gönder","Gelsin","Kodları","Durmasın"};//String tipinde dizi
        
        System.out.println(b[2] + "," + a[3] + "," + stri[2]);//cıktı 80, 6, kodları olmsı gerek 
        
        int arr[]={1,5,8,9,6,2,10,55,56,80};
        for(int i=0;i<arr.length;i++){//length dizinin uzunluğunu garantilemek için kullandık
            System.out.println(arr[i]);
        }
        //bir dizideki en küçük elamanı bulma
        int c[]={12,58,56,23,57,47,17,37,81,1,-13,-56};
       int sakla=c[0];
        for(int i=0;i<c.length;i++){
            if(sakla> c[i]){
                sakla=c[i];
        }
        }
            System.out.println(sakla);
            
            
    
        //en büyük bulma(elamı)
        int v[]={20,56,21,46,23,80,-13,-24};
        int ilk=v[0];
        for(int k=0;k<v.length;k++){
            if( ilk<v[k]){
                ilk=v[k];
            }
        
        }
        System.out.println(ilk);
        
        /*
        //ÇOK BOYUTLU DİZİLER
        int ar[][]={{5,6,4,8},{56,24,13,80},{46,17,19,34}};
        for(int o=0;o<3;o++){
            for(int j=0;j<4;j++){
                System.out.print(ar[o][j] + "");
            }
            System.out.println();
        } */
        
        
        // DİZİLERİ(MATRİX) TOPLAMA
        int dizi1[][]={{1,2,3,4,},{8,6,2,3},{10,4,6,3}};
        int dizi2[][]={{4,3,2,1},{5,6,7,8},{10,2,3,4}};
        int dizi3[][]=new int[3][4];
        for(int t=0;t<3;t++){
            for(int d=0;d<4;d++){
                dizi3[t][d]=dizi1[t][d] + dizi2[t][d];
                System.out.print(dizi3 +  ""); 
                        
        }
        System.out.println();
        }
        
    
    
    
    
    
    
    
    }
      
       
    
}

            
            
        ________________________________________________________________________________________________________________________    
            
            // DİZİNİN ELAMANLARINI TEK Mİ ÇİFT Mİ ? DİYE EKRANA YAZMA
            
            
            
            
            package rastgelesayıuretme;

import java.util.Random;
public class RastgeleSayıUretme {
    
    public static void main(String[] args) {
       /*
        Random ran=new Random();
        int a=ran.nextInt(5);
        System.out.println(a);
        */
      int dizi[]={12,13,14,54,6,4,3,5,67,78,89,80,86,123,3445,56,};
      System.out.print("çift sayılar:");
      for(int i=0;i<dizi.length;i++){
      if(dizi[i]%2==0){
      System.out.print(dizi[i]+" ");
          
      
      }
      
      }
      System.out.println();
     System.out.print("tek sayılar:");
     for(int i=0;i<dizi.length;i++){
     if(dizi[i]%2==1){
         System.out.print(dizi[i]+" ");
     
     }
     
     }
      
      
      
        
        
        
    }
    
}
 
  
   
    
     /////////////////////////////////////////////////////////////
    _______________________________________________________________ 
     
     PALİNDROM SAYI BULMA
     
     package alıştırma;

import java.util.Scanner;
public class Alıştırma {

    
    public static void main(String[] args) {
        Scanner scan=new Scanner (System.in);
        for(;;){
        System.out.println("lütfen palindrom oduğunu düşündüğünüz tam sayısını giriniz");
        int palindrom=scan.nextInt();
        int ilkdeger=palindrom;
        int sondeger=0;
        while(palindrom>0){
            sondeger=sondeger*10 + palindrom%10;
        palindrom= palindrom /10;
        
        }
      
        if(ilkdeger==sondeger)
            System.out.println(ilkdeger+ " sayısı palindrom sayıdır");
                
    else
            System.out.println(ilkdeger +" sayısı palindrom sayı değil");
        
        
        }
    }

    
    }
    
________________________________________________________________________________________________________________
     &&&&&&&&&&&&&&&&&&&&&&&++&&&&&&&&&&&&&&&&&&^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^&&&&&&&&&&/((((((((()>
     
     
     
     
package mukemmelsayı;

import java.util.Scanner;
public class MukemmelSayı{

    
    public static void main(String[] args) {
        Scanner scan=new Scanner (System.in);
        for(;;){
        System.out.println( "lütfen sayıyı giriniz");
        int sayi=scan.nextInt();
        int sayac=0;
        
        System.out.print(" bölen sayılar: " );
        for(int i=1;i<sayi;i++){
        if(sayi%i==0){
        System.out.print(i +" " );
        
        sayac+=i;
        }
        
        
        }
        
        if(sayac==sayi)
            System.out.println(sayi+" sayısı mükemmel sayıdır");
        
        else
            System.out.println(sayi +"sayısı mükemmel değil");
                
        }      
        
        
    }

    
    }
    


%%%%%%%%%%%%%%%%%%%%%%%%%%%%%&&&&&&&&&&&&&&&&&&&&&///////////////////////(((((((((((((((((((((((((()))))))))))))))))))))))))))))))
      
      
      package alıştırma;

import java.util.Scanner;
public class Alıştırma {

    
    public static void main(String[] args) {
        Scanner scan=new Scanner (System.in);
        for(;;){
        System.out.println("lütfen palindrom olduğunu düşündüğünüz kdelimeyi giriniz");
        String ilkkelime=scan.nextLine();
        String sonkelime="";
        
         for(int i=(ilkkelime.length()-1);i>=0;i--)
             sonkelime+=ilkkelime.charAt(i);
         if(sonkelime.equals(ilkkelime))
             System.out.println("palindrom kelime");
         else
             System.out.println("palindrom kelime değil");
        }
    }
    }
    
   ^^^^^^^^^^^^^^^^^^^^+++++++++++++++++%%%%%%%%%%%%%%%%%%%%%%%&&&&&&&&&&&&&&&&&&&///////////////>(((((((((((((^ééééééééééééééééééé!!!!!!!!!!!'''''''''^^^^^^^^^^

        // sını oluşruma kutunun hacmini hesaplama
       package alıştırma;

import java.util.Scanner;

 class Kutu{
     int en;
 int boy;
 int yükseklik;
 void TestKutu(int en,int boy,int yükseklik){
 
 int hacim=en*boy*yükseklik;
 System.out.println(hacim);
 }
 }
public class Alıştırma {
 
    public static void main(String[] args) {
        Scanner scan=new Scanner(System.in);
        System.out.println("hacminiz hesaplamak istediğiniz kotunun boy,en ve yüksekliğini giriniz");
        int en=scan.nextInt();
        int boy=scan.nextInt();
        int yükseklik=scan.nextInt();
        Kutu hacim= new Kutu();
        hacim.TestKutu(en,boy,yükseklik);
        
        
        
}
   

        
    
    }
    
    
    &&&&&&&&&&&&&&%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%MR%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
    
    // ÜST SINIFLARDAN ALT SINIF TÜRETME 
      
      package alıştırmalar2;

class Telefon{
    public Telefon(){// yapıcılar nesne oluşturulduğu anda çalışmaya başlar
    System.out.println("Telefon sınıfının yapıcısı");
    }
public Telefon(int b){
System.out.println("paremetreli yapı");
}
}
    class AkilliTelefon extends Telefon{
     public AkilliTelefon(){
     System.out.println("AkilliTelefon sınıfının yapıcısı");
     }}
    class cepTelefonu extends Telefon{
        public cepTelefonu(){
        System.out.println("cepTelefonu sınıfının yapıcısı");
        }}
    class Nokia extends cepTelefonu{
    public Nokia(){
    System.out.println("Nokia sınıfının yapıcısı");
    }
    }
    class NokiaA1 extends Nokia{
        public NokiaA1(){
        System.out.println("bu son kısımdı şimdi kaybol");
        }
    
    }

public class Alıştırmalar2 {

    
    
    
            
    public static void main(String[] args) {
       
        Telefon n1=new Telefon(5);
        
        NokiaA1 n=new NokiaA1();
                
                
    
    
   }
    
}
 
 
 &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&
  // NESNEYE YÖNELİK PROGRAMLAMA
  
  
package alıştırma;

import java.util.Scanner;
 class Sinif{
       
    String renk;//durum(özellik) diyer bir değişle attribute. KENDİSİ BİR NESNE DEĞİŞKENDİR SONRADAN ATANIR
    
    int boy;//durum(özellik) diyer bir değişle attribute
    
    int yas;//durum(özellik) diyer bir değişle attribute
    static int genelKod=00101223;//SINIF DEĞİŞKENİ diyer bir isimle STATİC değişken tüm nesler için ortaktır ve direkt değeri alır
    static int alanKod;// bu değeri son nesne için değiştirsek diğer tüm nesler bu  yeni değeri alır.
     void yukariGit()//durum/davranış/metod(actions)
     {
         System.out.println("yukarı gidiyor");
     }
    
     int metod(int n1,int n2,int n3){
     return n1*n2*n3;
     }
    }
 
public class Alıştırma{
    
    
 
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        
        Sinif nesne= new Sinif();// nesneyi oluşturduk
        
        nesne.renk="siyah";//nesnenin renk özelliğne değer atadık
        
        System.out.println(nesne.renk);// ekrana yazdırdık
        nesne.yukariGit();//metodu yani actions(davranışı) cağırdık ve doğasında olanı yapar
        
        // nesnein metodunu direkt çağırma veya bir değere ekleme
        int carpim=nesne.metod(2, 5, 8);
        System.out.println(nesne.metod(2,5,8) + carpim);
        
}
   

        
    
    }
    

    %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
    
    // overriding
    
    package javaapplication31;
 
class SinifA{

protected int sayi=6;
public String ad="kaos";
public String metod(){
    return ad+sayi;

}
}
class SinifB extends SinifA{

    public String metod(){
    return ad+sayi+ad+sayi;
    }

}

public class JavaApplication31 {

    
    public static void main(String[] args) {
       SinifB  nesne=new SinifB();
       System.out.println(nesne.metod());
        
    }
    
}

       
