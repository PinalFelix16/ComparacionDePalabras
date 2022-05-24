# ComparacionDePalabras
Comparar dos palabras y decir si son iguales o no

package CicloMIentras;
import javax.swing.JOptionPane;

public class Ecuals
{
   public static void main (String arg[]){
       
       String pal=" ",pal1=" ",paln=" ",pala=" ",Num=" ",igua=" ", palai=" ",palani=" ";
       int n=1,palan=0,palann=0,numem=0,totalpal=0,totpi=0;
       
       Num=JOptionPane.showInputDialog("Dame el numero de palabras a comparar");
       
       numem=Integer.parseInt(Num);
       while(n<=numem){
           pal=JOptionPane.showInputDialog("dame la palabra a comparar N*" + n);
           pal1=JOptionPane.showInputDialog("dame la palabra con la que deseas comparar");
           paln=" ";
           pala=" ";
           
           if(pal.equalsIgnoreCase(pal1))
           {
               JOptionPane.showMessageDialog(null,"las palabras son iguales");
               palai=pal+" y "+pal1+"\n";
               totpi+=+1;
            }
            else
            {
                JOptionPane.showMessageDialog(null,"las palabras son diferentes");
                palai=pal+" y "+pal1+"\n";
                totalpal+=+1;
            }
            igua="las palabras que son iguales son : "+palai+"\n";
        }
        JOptionPane.showMessageDialog(null,
        "numero de palabras a comparar son : "+Num+"\n"+
        "las palabras iguales son: "+totpi+"\n"+palai+"\n"+
        "las palabras diferentes son ; "+totalpal+"\n"+palani);
    }
}
