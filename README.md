# Practica2.FundamentosYSintaxisDelLenguaje
Practica 2. Fundamentos Y Sintaxis Del Lenguaje - Hernández Rubio Dana Valeria
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package poop2.dv;

/**
 *
 * @author Optiplex 780
 */
public class POOP2DV {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        int a = 36; int b =55;
        System.out.println("a= " + a);
        System.out.println("b= " + b);
        /*******************if*********************/
        if (a<b){
            System.out.println("a<b");
        }else{
            System.out.println("a>=b");
        }
        /*******************if*********************/
        if (a<b)
            System.out.println("a<b");
        else
            System.out.println("a>=b");
        /*************if- Método********************/
        if(f(a,b))
           System.out.println("f regesa true");
        else
           System.out.println("f regresa false");
        /*************if-else**************************/
        if(a<b)
            System.out.println("a < b");
        else if (a<=b)
            System.out.println("a<=b");
        else
             System.out.println("a > b");
        /******************************swich*******************/
        KeyboardInput teclado = new KeyboardInput();
        System.out.println("Escriba un numero entre 1 y 7");
        
        int dia = teclado.readInteger();
        switch(dia){
            case 1:
              System.out.println("Lunes");  
              break;
            case 2:
                System.out.println("Martes");
                break;
            case 3:
                System.out.println("Miercoles");
                break;
            case 4:
                System.out.println("Jueves");
                break;
            case 5:
                System.out.println("Viernes");
                break;
            case 6:
                System.out.println("Sabado");
                break;
            case 7:
                System.out.println("Domingo");
                break;
            default:
                System.out.println(dia + " No es un dia de la semana");
        }
        /***********************for**********************/
        int var = 5;
        int[] x = new int[var]; 
        for (int i = 0; i < var; i++){
            x[i] = i;
            System.out.println(x[i]);
        }
         System.out.println("Ahora viene el segundo for");
         for (int i = 0; i < var; i++)
            System.out.println(x[i]);
        System.out.println("Hola");  
        /***********************while**********************/
        int i = 0;
        while(i<var){
            System.out.println("Contando hacia arriba " + i); 
            //i = i+1;
            i++;
        }
        
        System.out.println(i); 
        
        while(i>0){
           System.out.println("Contando hacia abajo " + i); 
           //i = i -1;
           i--;
        }
        System.out.println(i);
         /***********************do-while**********************/
         do{
             System.out.println("Contando hacia abajo " + i);
             i--;
         }while(i>0);
         System.out.println(i);
          /***********************contnue**********************/
          int s= 5;
          String k = "6";
          int z = 5+Integer.parseInt(k);
          System.out.println("Z es iguale a " +z);
          
         for(int j = 0; j<10; j++){
              System.out.println("Escoja un numero: ");
              float numero = teclado.readFloat();
              if(numero == 0){
                  System.out.println("Division entre cero");
                  continue;
              }
              System.out.println("100/"+ numero + " = " + 100.0/numero);// el .0 en el 100 vuelve el numero a flotante, tambien puede ser 100f
         } 
         System.out.println("bandera");
    }
    public static boolean f(int x, int y){
        return (x<y);
    }
}
