```c
#include <stdio.h>
void completarMatrices (int a[2][3]);
void sumaMatrices (int b[2][3], int c[2][3], int d[2][3]);
void restaMatrices (int b[2][3], int c[2][3], int d[2][3]);
void multiplicacionMatrices (int b[2][3], int c[2][3], int d[2][3]);
void mostrarResultado(int d[2][3]);
// Función principal
int main(){
    int matriz1[2][3];
    int matriz2[2][3];
    int matrizResultado[2][3];
    // Ingreso de datos de funciones 
    printf("Primera Matriz\n");
    completarMatrices(matriz1);
    printf("Segunda Matriz\n");
    completarMatrices(matriz2);

    //Suma
    sumaMatrices(matriz1, matriz2, matrizResultado);
    printf("SUMA\n");
    mostrarResultado(matrizResultado);

    //Resta
    restaMatrices(matriz1, matriz2, matrizResultado);
    printf("RESTA\n");
    mostrarResultado(matrizResultado);

    //Multiplicacion
    multiplicacionMatrices(matriz1, matriz2, matrizResultado);
    printf("MULTIPLICACION\n");
    mostrarResultado(matrizResultado);
    return 0;
}
// Funcion que permite ingresar los datos de las matrices 
void completarMatrices (int a[2][3]){
    int i, j;
    for(i=0; i<2; i++){
        for(j=0; j<3;j++){
            printf("Ingrese el valor en la posicion %i %i\n", i, j);
            scanf("%i", &a[i][j]);
            getchar();
        }
    }
    
}
// Funcion que suma dos matrices 
void sumaMatrices (int b[2][3], int c[2][3], int d[2][3]){
    int i, j; 
    for(i=0; i<2; i++){
        for(j=0; j<3;j++){
            d[i][j]=b[i][j]+c[i][j];
        }
    }
    
}
// Funcion que resta dos matrices
void restaMatrices (int b[2][3], int c[2][3], int d[2][3]){
    int i, j; 
    for(i=0; i<2; i++){
        for(j=0; j<3;j++){
            d[i][j]=b[i][j]-c[i][j];
        }
    }
    
}
// Funcion que multiplica los elementos de dos matrices 
void multiplicacionMatrices (int b[2][3], int c[2][3], int d[2][3]){
    int i, j; 
    for(i=0; i<2; i++){
        for(j=0; j<3;j++){
            d[i][j]=b[i][j]*c[i][j];
        }
    }
    
}
// Función que permite mostrar los resultados 
void mostrarResultado(int d[2][3]){
    int i, j;
    for(i=0; i<2; i++){
        for(j=0; j<3; j++){
            printf("El valor en la posicion %i%i es: %i\n", i, j, d[i][j]);
        }
    }
}
```
