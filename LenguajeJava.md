```java
import java.util.Scanner;
public class OperacionesMatriz{
    public static void main(String[] args){
        Scanner entrada = new Scanner(System.in);
        int[][] matriz1= new int [2][3];
        int[][] matriz2= new int [2][3];
        int[][] matrizResultado= new int [2][3];

        // Pedir valores de matrices 
        System.out.println("Primera Matriz");
        completarMatriz(matriz1, entrada);
        System.out.println("Segunda Matriz");
        completarMatriz(matriz2, entrada);

        // Suma
        sumaMatrices(matriz1, matriz2, matrizResultado);
        System.out.println("SUMA"); 
        mostrarResultado(matrizResultado);

        // Resta
        restaMatrices(matriz1, matriz2, matrizResultado);
        System.out.println("RESTAR"); 
        mostrarResultado(matrizResultado);

        // Multiplicacion
        multiplicacionMatrices(matriz1, matriz2, matrizResultado);
        System.out.println("MULTIPLICACION"); 
        mostrarResultado(matrizResultado);

        entrada.close();
    }
    public static void completarMatriz (int[][] matriz, Scanner entrada){
        for(int i = 0; i < matriz.length; i++){
            for( int j=0; j< matriz[i]. length; j++){
                System.out.println("Ingrese el valor en la posicion ["+ i +"] ["+ j +"]:");
                matriz[i][j]=entrada.nextInt();

            }
        }
    }
    public static void sumaMatrices (int[][] matriz1, int[][] matriz2, int[][]matrizResultado){
        for(int i = 0; i<matriz1.length; i++){
            for(int j = 0; j<matriz1[i].length; j++){
                matrizResultado[i][j]=matriz1[i][j]+matriz2[i][j];
            }
        }
    }
    public static void restaMatrices (int[][] matriz1, int[][] matriz2, int[][]matrizResultado){
        for(int i = 0; i<matriz1.length; i++){
            for(int j = 0; j<matriz1[i].length; j++){
                matrizResultado[i][j]=matriz1[i][j]-matriz2[i][j];
            }
        }
    }
    public static void multiplicacionMatrices (int[][] matriz1, int[][] matriz2, int[][]matrizResultado){
        for(int i = 0; i<matriz1.length; i++){
            for(int j = 0; j<matriz1[i].length; j++){
                matrizResultado[i][j]=matriz1[i][j]*matriz2[i][j];
            }
        }
    }
    public static void mostrarResultado(int[][] matriz){
        for(int i = 0; i<matriz.length; i++){
            for(int j = 0; j<matriz[i].length; j++){
                System.out.println("El valor en la posicion ["+ i +"]["+ j +"] es: " + matriz[i][j] );
            }
        }
    }
}
```
