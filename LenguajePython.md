```python
# Funcion que permite completar las matrices
def completar_matriz(matriz, nombre_matriz):
    print(f"\n--- {nombre_matriz} ---")
    for i in range(len(matriz)):
        for j in range(len(matriz[i])):
            matriz[i][j] = int(input(f"Ingrese el valor en la posicion [{i}][{j}]: "))

# Funcion que permite sumar dos matrices 
def suma_matrices(matriz1, matriz2, matriz_resultado):
    for i in range(len(matriz1)):
        for j in range(len(matriz1[i])):
            matriz_resultado[i][j] = matriz1[i][j] + matriz2[i][j]

# Funcion que permite restar dos matrices 
def resta_matrices(matriz1, matriz2, matriz_resultado):
    for i in range(len(matriz1)):
        for j in range(len(matriz1[i])):
            matriz_resultado[i][j] = matriz1[i][j] - matriz2[i][j]

# Funcion que permite multiplicar matrices 
def multiplicacion_matrices(matriz1, matriz2, matriz_resultado):
    for i in range(len(matriz1)):
        for j in range(len(matriz1[i])):
            matriz_resultado[i][j] = matriz1[i][j] * matriz2[i][j]

# Funcion que muestra los resultados de las operaciones 
def mostrar_resultado(matriz):
    for i in range(len(matriz)):
        for j in range(len(matriz[i])):
            print(f"El valor en la posicion [{i}][{j}] es: {matriz[i][j]}")

# Funcion principal 
def main():
    matriz1 = [[0 for _ in range(3)] for _ in range(2)]
    matriz2 = [[0 for _ in range(3)] for _ in range(2)]
    matriz_resultado = [[0 for _ in range(3)] for _ in range(2)]

    completar_matriz(matriz1, "Primera Matriz")
    completar_matriz(matriz2, "Segunda Matriz")

    # Suma
    suma_matrices(matriz1, matriz2, matriz_resultado)
    print("\n=== SUMA ===")
    mostrar_resultado(matriz_resultado)

    # Resta
    resta_matrices(matriz1, matriz2, matriz_resultado)
    print("\n=== RESTA ===")
    mostrar_resultado(matriz_resultado)

    # Multiplicacion
    multiplicacion_matrices(matriz1, matriz2, matriz_resultado)
    print("\n=== MULTIPLICACION ===")
    mostrar_resultado(matriz_resultado)

if __name__ == "__main__":
    main()
```
