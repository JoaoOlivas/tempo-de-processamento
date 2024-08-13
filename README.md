public class Funcoes {

    public int f1(int n) {
        int r = 0;
        for (int i = 0; i < n; i++) {
            r = r + 1;
        }
        return r;
    }

    public int f2aux(int n) {
        int r = 0;
        for (int i = 1; i < n; i++) {
            for (int j = 1; j < n; j++) {
                r = r + 1;

            }
        }
        return r;
    }

    public int f2(int n) {
        int r = 0;
        for (int i = 1; i < n; i++) {
            for (int j = i + 1; j < n; j++) {
                r = r + 1;

            }
        }
        return r;
    }

 

    public int f4(int n) {
        int r = 0;
        for (int i = 1; i < n; i++) {
            for (int j = i; j < 2 * i; j++) {
                for (int k = i; k < j; k++) {
                    r = r + 1;
                }
            }
        }
        return r;

    }

    public int f5(int n) {
        int r = 0;
        for (int i = 1; i < n; i++) {
            for (int j = i; j < i + 3; j++) {
                for (int k = i; k < j; k++) {
                    r = r + 1;
                }
            }
        }
        return r;
    }

}
----------------------------------------------------------------codigo 1 --------------------------------------------------------------------


import java.util.Scanner;

public class App {


    public static void main(String[] args) {

        Scanner teclado= new Scanner(System.in);
        
System.out.print("Digite um numero de 1 a 4 para decidir a sua operação" );

int variavel = teclado.nextInt();


if (variavel == 1 ) { 

Funcoes f = new Funcoes();

        for(int i=1; i<300; i+=10){
        
            int r = f.f1(i);
            
            System.out.println(i+";"+r);
            
        }
        
    }
    
 if (variavel == 2 ) { 
 
Funcoes f = new Funcoes();

        for(int i=1; i<300; i+=10){
        
            int r = f.f2(i);
            
            System.out.println(i+";"+r);
            
        }
        
    }
    
    if (variavel == 3 ) { 
    
Funcoes f = new Funcoes();

        for(int i=1; i<300; i+=10){
        
            int r = f.f4(i);
            
            System.out.println(i+";"+r);
            
        }
        
    }
    
    if (variavel == 4 ) { 
    
Funcoes f = new Funcoes();

        for(int i=1; i<300; i+=10){
        
            int r = f.f5(i);
            
            System.out.println(i+";"+r);
            
        }
        
    }
    
    }   
    
}

---------------------------------------------------------------------codigo 2-------------------------------------------------------------------------------
