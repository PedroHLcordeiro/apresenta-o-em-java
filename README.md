// apresenta-o-em-java
// um apresentação em código que fiz em java

import java.util.Scanner;
public class Principal {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Ficha pessoal = new Ficha();

        pessoal.nome = "Pedro";
        pessoal.NomeDoCurso = "Defesa cibernética";
        pessoal.NomeFaculdade = "FIAP";
        pessoal.anoDeMatricula = 2023;

        System.out.println(pessoal.nome);
        System.out.println(pessoal.NomeFaculdade);
        System.out.println(pessoal.NomeDoCurso);
        System.out.println(pessoal.anoDeMatricula);

        System.out.println("\nOlá, meu nome é Pedro e sou estudante de cybersecurity, além disso " +
                "sou um entusiasta de tecnologia de modo geral +_+");

        System.out.println("""
                digite 1
                para saber a Linguagem de programação principal;
                a Linguagem de programação secundária;
                e para saber a area que mais estudei em cyber;
                """);

        int opcao = scanner.nextInt();
        // confundi a ordem do scanner e a lógica dele, estudar mais a respeito
        switch (opcao) {
            case 1:
                System.out.println("Linguagem de programação principal: Java");
                System.out.println("Linguagem de programação secundária: Python");
                System.out.println("Área que mais estudei em cybersecurity: Web");
                break;
        // enfrentei um problema na quebra de código nessa parte
            default:
                System.out.println("Opção inválida.");
        }
    }
}
// fiz essa parte em outra janela
public class Ficha {
    String nome;
    String NomeDoCurso;
    String NomeFaculdade;
    int anoDeMatricula;

}
