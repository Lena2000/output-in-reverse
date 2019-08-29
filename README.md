package javaapplication22;

import java.util.Scanner;

/**
 *
 * @author LENOVO
 */
public class JavaApplication22 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
          Scanner sc = new Scanner(System.in);
         
        int i;
        System.out.println("Input size of array: ");
        int kol=sc.nextInt();
        int[]array=new int[kol];
       
        System.out.println("Input elements of array: ");
        for( i=0; i<kol; i++)
           array[i]=sc.nextInt();
        
      
        for(i=0; i<( kol/2); i++){
            int b=array[i];
            array[i]=array[kol-1-i];
            array[kol-1-i]=b;
    }
    System.out.println("Result");
        for( i=0; i<kol; i++)
            System.out.print(array[i]+" ");
}
}
