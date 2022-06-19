
package Semana05

import java.util.Scanner;

public class Practica5 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        int dni=0;
        double sueldo_operario=0,sueldo_a_cobrar;
        String nombre_operario;
        Scanner sc=new Scanner(System.in);
          System.out.println("Ingrese el nombre del operario: ");
          nombre_operario=sc.next();
          System.out.println("Ingrese el número de DNI del operario: ");
          dni=sc.nextInt();
          System.out.println("Ingrese el sueldo del operario: ");
          sueldo_operario=sc.nextDouble();
          double salud=sueldo_operario*0.03;
          double ali_y_viv=sueldo_operario*0.15;
          double descuento=salud+ali_y_viv;
          sueldo_a_cobrar=sueldo_operario-descuento;
          System.out.println("-----EMPRESA DONOFRIO-----");
          System.out.println("El operario de la Empresas Donofrio: "+nombre_operario
                  +"\n"+"Su número de DNI es: "+dni
                  +"\n"+"Su descuento total es: S/. "+descuento
                  +"\n"+"Su sueldo a cobrar es: S/. "+sueldo_a_cobrar);
    }
    
}
