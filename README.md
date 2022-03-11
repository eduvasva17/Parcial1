package parcialxdxd;

import java.util.Scanner;
/**
 *
 * @author edx
 */
public class Parcialxdxd {

    /**
     * @param args the command line arguments
     */
static Scanner scanner = new Scanner(System.in);    
    
public static double promediar_estudiante(double n1, double n2, double n3){
    double promedio = (n1*0.3)+ (n2*0.25)+(n3*0.45);
    return promedio;
}
    
    public static void main(String[] args) {
        // TODO code application logic here
        System.out.println("Ingrese el nombre del estudiante");
        String nombre = scanner.nextLine();
        System.out.println("Ingrese el nombre del codigo"); 
        String codigo = scanner.nextLine();
        
        System.out.println("Ingrese la primera nota "); 
        double nota1 = scanner.nextDouble();
        System.out.println("Ingrese la segunda nota "); 
        double nota2 = scanner.nextDouble(); 
        System.out.println("Ingrese la tercera nota "); 
        double nota3 = scanner.nextDouble(); 
        
        System.out.println("El estudiante "+nombre+" con codigo "+codigo+" tiene un promedio de: "+promediar_estudiante(nota1, nota2, nota3) );
    }
    
}
