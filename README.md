package com.mycompany.jogodoluigi;
import java.random; 
/**
 *
 * @author aluno.cyber
 */

public class JogoDoLuigi {

    public static void main(String[] args) {
        
        Boss boss = new Boss();
        Luigi luigi = new Luigi();
        Princesa princesa = new Princesa();
        Combate combate = new Combate();

        Random entrada = new Random();
  int numero = entrada.nextInt(10);
   switch (numero) {
     case 1 -> System.out.println("O número escolhido foi: 1.");
     case 2 -> System.out.println("O número escolhido foi: 2.");
     case 3 -> System.out.println("O número escolhido foi: 3.");
     case 4 -> System.out.println("O número escolhido foi: 4.");
     case 5 -> System.out.println("O número escolhido foi: 5.");
     case 6 -> System.out.println("O número escolhido foi: 6.");
     case 7 -> System.out.println("O número escolhido foi: 7.");
     case 8 -> System.out.println("O número escolhido foi: 8.");
     case 9 -> System.out.println("O número escolhido foi: 9.");
     default -> System.out.println("O número escolhido foi: 10.");
   }
      
        while(luigi.Pontos != boss.Pontos ){
            
        }
    }
}
////////////////


package com.mycompany.jogodoluigi;

/**
 *
 * @author alunovdi
 */
public class Luigi {
    
   public String CorDaCapa;
   public String Ocupação;
   public double Tamanho;
   public int Vida;
   public double Peso;
   public int Pontos;
   
    public Luigi() {
        this.CorDaCapa = "amarela";
        this.Ocupação = "encanador";
        this.Tamanho = 1.75;
        this.Vida = 100;
        this.Peso = 89.8;
        this.Pontos = 0;
    }
    
}

////////////////////////


package com.mycompany.jogodoluigi;

/**
 *
 * @author alunovdi
 */
public class Tela {
    
}


////////////////


package com.mycompany.jogodoluigi;

/**
 *
 * @author alunovdi
 */
public class Bot {
    
}

////////////////


package com.mycompany.jogodoluigi;

/**
 *
 * @author alunovdi
 */
public class Boss {
    
}


///////////////


package com.mycompany.jogodoluigi;

/**
 *
 * @author alunovdi
 */
public class Combate {
   
    Luigi luigi = new Luigi();
    
    public void Combate (boolean luta){
        if (luta == true){
        luigi.Pontos -= 2;
        }
        }
    }



////////////////


/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Class.java to edit this template
 */
package com.mycompany.jogodoluigi;

/**
 *
 * @author alunovdi
 */
public class Princesa {
    Luigi luigi = new Luigi();
    
   
    public void Salvar(boolean princesaSalva ){
       
        if (princesaSalva == true) {
          System.out.println("true");
           luigi.Pontos+=10;
            System.out.println(luigi.Pontos);}
         
        else{
              System.out.println("false");
        }
    }
}
