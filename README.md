Exercício 1 
import java.util.Scanner;

public class main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        // Variáveis para armazenar as maiores notas e as respectivas matrículas
        int matricula1 = 0, matricula2 = 0;
        double maiorNota = Double.NEGATIVE_INFINITY, segundaMaiorNota = Double.NEGATIVE_INFINITY;

        for (int i = 0; i < 100; i++) {
            System.out.print("Digite a matrícula do aluno " + (i + 1) + ": ");
            int matricula = scanner.nextInt();

            System.out.print("Digite a nota do aluno " + (i + 1) + ": ");
            double nota = scanner.nextDouble();

            // Verifica se a nota atual é maior que a maior nota encontrada
            if (nota > maiorNota) {
                segundaMaiorNota = maiorNota; // Atualiza a segunda maior nota
                matricula2 = matricula1; // Atualiza a matrícula da segunda maior nota
                maiorNota = nota; // Atualiza a maior nota
                matricula1 = matricula; // Atualiza a matrícula da maior nota
            } 
            // Verifica se a nota atual é maior que a segunda maior nota encontrada
            else if (nota > segundaMaiorNota) {
                segundaMaiorNota = nota; // Atualiza a segunda maior nota
                matricula2 = matricula; // Atualiza a matrícula da segunda maior nota
            }
        }

        // Imprime as duas maiores notas e as respectivas matrículas
        System.out.println("Maior Nota: " + maiorNota + ", Matrícula: " + matricula1);
        System.out.println("Segunda Maior Nota: " + segundaMaiorNota + ", Matrícula: " + matricula2);
            }
}
Exercício 2 


import java.util.Scanner;

public class main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
         
        System.out.print("Digite o valor de n: ");
        int n = scanner.nextInt();
        
        for (int i = 1; i <= n; i++) {
            int valor = (i + 1) / 2; // Calcula o valor da série
            // Imprime o número apropriado com a frequência correta
            for (int j = 0; j < (i % 2 == 0 ? 2 : 1); j++) {
                System.out.print(valor + " ");
            }
        }
   Exercício 3 
   
   import java.util.Scanner;

public class main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
    
        System.out.print("Digite o sexo (1 - feminino, 2 - masculino): ");
        int sexo = scanner.nextInt();
        
        System.out.print("Digite o tempo de contribuição em 2019 (anos): ");
        int tempoContribuicao = scanner.nextInt();
        
        System.out.print("Digite a idade em 2019: ");
        int idade = scanner.nextInt();
        
        int pontosMinimosHomem = 96;
        int pontosMinimosMulher = 86;
        int pontosMaximosHomem = 105;
        int pontosMaximosMulher = 100;
Não finalizado! 
