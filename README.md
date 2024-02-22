# VerificaNumeroPerfeito


package numeroperfeito;
 
import java.util.Scanner;

public class NumeroPerfeito {

   
    public static void main(String[] args) {
        
     Scanner Scanner = new Scanner (System.in);  
     
        System.out.println("Digite um número inteiro positivo:");
        int numero= Scanner.nextInt();
        if(verificanumeroperfeito(numero)){
            System.out.println(numero + " é um numero perfeito.");
        }else{
            System.out.println(numero + " nâo é um número perfeito.");
     }
        // fecha Scanner
        Scanner.close();
     }
    public static boolean verificanumeroperfeito( int numero){
        int somadosdivisores =0;
        for (int i =1; i< numero; i++){
            if(numero%i==0){
                somadosdivisores+=i;
                
            }
        }
        return somadosdivisores==numero;
    }
    
}
