import java.util.Scanner;

/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author dell
 */
public class Principal {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner input = new Scanner(System.in);
        
        System.out.println("¿Qué operación quieres ejecutar?");
        String sOperacion;
        sOperacion = input.nextLine();
        
        System.out.println("Introduce el Numerador de la Primera Fracción");
        double rNumerador1;        
        rNumerador1 = input.nextDouble();
        
        System.out.println("Introduce el Denominador de la Primera Fracción");
        double rDenominador1;
        rDenominador1 = input.nextDouble();
        
        System.out.println("Introduce el Numerador de la Segunda Fracción");
        double rNumerador2;        
        rNumerador2 = input.nextDouble();
        
        System.out.println("Introduce el Denominador de la Segunda Fracción");
        double rDenominador2;
        rDenominador2 = input.nextDouble();

        if (sOperacion.equals("suma")) {
            double numeradorSuma;
            double denominadorSuma;
            
            numeradorSuma = rNumerador1 * rDenominador2 + rNumerador2 * rDenominador1;
            denominadorSuma = rDenominador1 * rDenominador2;
            System.out.println("La Suma da: "+numeradorSuma+"/"+denominadorSuma);
        } else {
            if (sOperacion.equals("resta")) {
                double numeradorResta;
                double denominadorResta;
                
                numeradorResta = rNumerador1 * rDenominador2 - rNumerador2 * rDenominador1;
                denominadorResta = rDenominador1 * rDenominador2;
                System.out.println("La Resta da: "+numeradorResta+"/"+denominadorResta);
            } else {
                if (sOperacion.equals("multiplicacion")) {
                    double numeradorMulti;
                    double denominadorMulti;
                    
                    numeradorMulti = rNumerador1 * rNumerador2;
                    denominadorMulti = rDenominador1 * rDenominador2;
                    System.out.println("La Multiplicación da: "+numeradorMulti+"/"+denominadorMulti);
                } else {
                    if (sOperacion.equals("division")) {
                        double numeradorDivision;
                        double denominadorDivision;
                        
                        numeradorDivision = rNumerador1 * rDenominador2;
                        denominadorDivision = rDenominador1 * rNumerador2;
                        System.out.println("La División da: "+numeradorDivision+"/"+denominadorDivision);
                    }
                }
            }
        }
    }
}
