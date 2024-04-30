# numpyBD


Open In Colab

# IMPORTAR NumPy
import numpy as np
     

# Crear una matriz bidimensional (matriz) de tamaño 3x3 con valores enteros consecutivos.
matriz = np.arange(1, 10).reshape(3, 3)
     

# Paso 1: CREACIÓN DE ARRARS
# Crear un array unidimensional (vector) con 5 elementos enteros de tu elección.
vector = np.array([1, 2, 3, 4, 5,6,7,8,9])
     

# Utilizar la función np.zeros() para crear una matriz de tamaño 2x4 llena de ceros.
matriz_zeros = np.zeros((2, 4))
     

# Utilizar la función np.ones() para crear una matriz de tamaño 3x2 llena de unos.
matriz_unos = np.ones((3, 2))
     

# Utilizar la función np.random.randint() para crear una matriz de tamaño 4x4 con números enteros aleatorios entre 0 y 10.
matriz_random = np.random.randint(0, 10, size=(4, 4))
     

# Paso 2: ACCESO A ELEMENTO
# Acceder al tercer elemento del vector creado en el paso 1.
tercer_elemento_vector = vector[2]
     

# Acceder al elemento en la segunda fila y segunda columna de la matriz creada en el paso 1.
elemento_2_2_matriz = matriz[1, 1]
     

# Paso 3: PROPIEDADES DE LOS ARRARYS
# Utilizar el atributo ndim para verificar la cantidad de dimensiones de la matriz creada en el paso 2.
dimensiones_matriz = matriz.ndim
     

# Utilizar el atributo shape para obtener la forma de la matriz creada en el paso 2.
forma_matriz = matriz.shape
     

# Utilizar el atributo size para obtener el tamaño total de la matriz creada en el paso 2.
tamaño_matriz = matriz.size
     

# Paso 4: OPERACIONES BÁSICAS
# Sumar dos matrices de tamaño 2x2 con valores aleatorios entre 0 y 10.
matriz_aleatoria_1 = np.random.randint(0, 10, size=(2, 2))
matriz_aleatoria_2 = np.random.randint(0, 10, size=(2, 2))
suma_matrices = matriz_aleatoria_1 + matriz_aleatoria_2
     

# Multiplicar dos matrices de tamaño 3x2 y 2x3 respectivamente.
matriz_3x2 = np.random.randint(0, 10, size=(3, 2))
matriz_2x3 = np.random.randint(0, 10, size=(2, 3))
multiplicacion_matrices = np.dot(matriz_3x2, matriz_2x3)
     

# Dividimos una matriz de tamaño 2x2 por otra matriz de tamaño 2x2, utilizando tanto la división por elementos como la multiplicación por la inversa.
matriz_dividida = np.random.randint(1, 10, size=(2, 2))
matriz_inversa = np.linalg.inv(matriz_dividida)
resultado_division = matriz_dividida / matriz_dividida
resultado_multiplicacion = np.dot(matriz_dividida, matriz_inversa)
     

# Paso 5: MANIPULACIÓN DE ARRAYS
# Utilizar la función reshape() para convertir el vector creado en el paso 2 en una matriz de tamaño 1x9.
vector_reshaped = vector.reshape(1, 9)

     

# Utilizar la función flatten() para convertir la matriz creada en el paso 2 en un vector unidimensional.
matriz_flattened = matriz.flatten()
     

# Paso 6: OPERACIONES ESTADÍSTICAS
# Calcular la suma de todos los elementos de la matriz creada en el paso 2.
suma_elementos_matriz = matriz.sum()
     

# Calcular la media de cada fila de la matriz creada en el paso 2.
media_filas_matriz = matriz.mean(axis=1)
     

# Paso 7: INTERACCIÓN Y REBANADO
# Imprimir la primera fila de la matriz creada en el paso 2.
primera_fila = matriz[0]
     

# Imprimir las primeras dos columnas de la matriz creada en el paso 2.
primeras_dos_columnas = matriz[:, :2]
     

# Paso 8: EJERCICIO ADICIONAL
# Definir una matriz de tamaño 4x4 con valores aleatorios.
matriz_adicional = np.random.randint(0, 100, size=(4, 4))
     

# Encontrar el valor máximo y mínimo de la matriz, así como su posición.
valor_maximo = matriz_adicional.max()
posicion_maximo = np.unravel_index(matriz_adicional.argmax(), matriz_adicional.shape)
valor_minimo = matriz_adicional.min()
posicion_minimo = np.unravel_index(matriz_adicional.argmin(), matriz_adicional.shape)
     

# IMPRIMIR RESULTADOS
print("Vector:", vector)
print("Matriz:\n", matriz)
print("Matriz de ceros:\n", matriz_zeros)
print("Matriz de unos:\n", matriz_unos)
print("Matriz aleatoria:\n", matriz_random)
print("Tercer elemento del vector:", tercer_elemento_vector)
print("Elemento en la segunda fila y segunda columna de la matriz:", elemento_2_2_matriz)
print("Dimensiones de la matriz:", dimensiones_matriz)
print("Forma de la matriz:", forma_matriz)
print("Tamaño total de la matriz:", tamaño_matriz)
print("Suma de matrices aleatorias:", suma_matrices)
print("Multiplicación de matrices:", multiplicacion_matrices)
print("División de matrices:", resultado_division)
print("Multiplicación por la inversa:", resultado_multiplicacion)
print("Vector reshaped:", vector_reshaped)
print("Matriz flattened:", matriz_flattened)
print("Suma de elementos de la matriz:", suma_elementos_matriz)
print("Media de cada fila de la matriz:", media_filas_matriz)
print("Primera fila de la matriz:", primera_fila)
print("Primeras dos columnas de la matriz:\n", primeras_dos_columnas)
print("Matriz adicional:\n", matriz_adicional)
print("Valor máximo:", valor_maximo, "en posición:", posicion_maximo)
print("Valor mínimo:", valor_minimo, "en posición:", posicion_minimo)
     
Vector: [1 2 3 4 5 6 7 8 9]
Matriz:
 [[1 2 3]
 [4 5 6]
 [7 8 9]]
Matriz de ceros:
 [[0. 0. 0. 0.]
 [0. 0. 0. 0.]]
Matriz de unos:
 [[1. 1.]
 [1. 1.]
 [1. 1.]]
Matriz aleatoria:
 [[3 3 1 0]
 [9 8 5 8]
 [5 9 8 7]
 [0 0 4 7]]
Tercer elemento del vector: 3
Elemento en la segunda fila y segunda columna de la matriz: 5
Dimensiones de la matriz: 2
Forma de la matriz: (3, 3)
Tamaño total de la matriz: 9
Suma de matrices aleatorias: [[13  9]
 [ 4  7]]
Multiplicación de matrices: [[ 6 50 34]
 [ 3 28 23]
 [ 9 77 55]]
División de matrices: [[1. 1.]
 [1. 1.]]
Multiplicación por la inversa: [[1.00000000e+00 2.77555756e-17]
 [0.00000000e+00 1.00000000e+00]]
Vector reshaped: [[1 2 3 4 5 6 7 8 9]]
Matriz flattened: [1 2 3 4 5 6 7 8 9]
Suma de elementos de la matriz: 45
Media de cada fila de la matriz: [2. 5. 8.]
Primera fila de la matriz: [1 2 3]
Primeras dos columnas de la matriz:
 [[1 2]
 [4 5]
 [7 8]]
Matriz adicional:
 [[ 7  9 17 31]
 [59  5 57 89]
 [91 62 89 43]
 [45 48 85 27]]
Valor máximo: 91 en posición: (2, 0)
Valor mínimo: 5 en posición: (1, 1)

# Definimos los nombres de las variables que queremos imprimir
variables_a_imprimir = [
    "vector", "matriz", "matriz_zeros", "matriz_unos", "matriz_random",
    "tercer_elemento_vector", "elemento_2_2_matriz", "dimensiones_matriz",
    "forma_matriz", "tamaño_matriz", "suma_matrices", "multiplicacion_matrices",
    "resultado_division", "resultado_multiplicacion", "vector_reshaped",
    "matriz_flattened", "suma_elementos_matriz", "media_filas_matriz",
    "primera_fila", "primeras_dos_columnas", "matriz_adicional",
    "valor_maximo", "posicion_maximo", "valor_minimo", "posicion_minimo"
]

# Imprimimos los resultados de forma compacta
for variable in variables_a_imprimir:
    valor_variable = locals().get(variable)
    if valor_variable is not None:
        print(f"{variable}: {valor_variable}")

     
vector: [1 2 3 4 5 6 7 8 9]
matriz: [[1 2 3]
 [4 5 6]
 [7 8 9]]
matriz_zeros: [[0. 0. 0. 0.]
 [0. 0. 0. 0.]]
matriz_unos: [[1. 1.]
 [1. 1.]
 [1. 1.]]
matriz_random: [[3 3 1 0]
 [9 8 5 8]
 [5 9 8 7]
 [0 0 4 7]]
tercer_elemento_vector: 3
elemento_2_2_matriz: 5
dimensiones_matriz: 2
forma_matriz: (3, 3)
tamaño_matriz: 9
suma_matrices: [[13  9]
 [ 4  7]]
multiplicacion_matrices: [[ 6 50 34]
 [ 3 28 23]
 [ 9 77 55]]
resultado_division: [[1. 1.]
 [1. 1.]]
resultado_multiplicacion: [[1.00000000e+00 2.77555756e-17]
 [0.00000000e+00 1.00000000e+00]]
vector_reshaped: [[1 2 3 4 5 6 7 8 9]]
matriz_flattened: [1 2 3 4 5 6 7 8 9]
suma_elementos_matriz: 45
media_filas_matriz: [2. 5. 8.]
primera_fila: [1 2 3]
primeras_dos_columnas: [[1 2]
 [4 5]
 [7 8]]
matriz_adicional: [[ 7  9 17 31]
 [59  5 57 89]
 [91 62 89 43]
 [45 48 85 27]]
valor_maximo: 91
posicion_maximo: (2, 0)
valor_minimo: 5
posicion_minimo: (1, 1)
