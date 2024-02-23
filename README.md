# Documentación de la función leer_carpeta(carpeta)
Descripción:

La función leer_carpeta(carpeta) lee todos los archivos .txt en una carpeta y los concatena en un solo DataFrame.

Parámetros:

carpeta: La ruta a la carpeta que contiene los archivos .txt.
Retorno:

Un DataFrame que contiene todos los datos de los archivos .txt en la carpeta.

Pasos a paso:

Recorrer los archivos de la carpeta: Se utiliza la función os.walk() para recorrer la carpeta especificada y obtener una lista de todos los archivos y subcarpetas.
Validar archivos .txt: Se comprueba si cada archivo en la lista tiene la extensión .txt.
Leer archivos .txt: Se utiliza la función open() para abrir cada archivo .txt en modo lectura.
Convertir archivos a DataFrame: Se utiliza la función pd.read_csv() para convertir cada archivo .txt en un DataFrame.
Agregar DataFrame a una lista: Se agrega cada DataFrame a una lista llamada DataFrame.
Concatenar DataFrames: Se utiliza la función pd.concat() para concatenar todos los DataFrames en la lista DataFrame en un solo DataFrame.
Retornar DataFrame: Se retorna el DataFrame final que contiene todos los datos de los archivos .txt en la carpeta.
Función os.walk():

La función os.walk() es una función de la biblioteca os que se utiliza para recorrer una carpeta y sus subcarpetas. La función devuelve un generador que produce una tupla para cada archivo o subcarpeta en la carpeta. La tupla contiene tres elementos:

Nombre de la carpeta: El nombre de la carpeta actual.
Lista de subcarpetas: Una lista de las subcarpetas en la carpeta actual.
Lista de archivos: Una lista de los archivos en la carpeta actual.
Contexto with:

El contexto with se utiliza para garantizar que los recursos se abran y cierren correctamente. En este caso, se utiliza el contexto with para abrir el archivo .txt y asegurarse de que se cierra correctamente después de que se haya leído.

Ejemplo de uso:

Python
carpeta = r"C:\Users\usuario\Desktop\Carpeta_con_archivos"
df = leer_carpeta(carpeta)

print(df.head())
Usa el código con precaución.
Salida:

   Columna1  Columna2  Columna3
0       Valor1      Valor2      Valor3
1       Valor4      Valor5      Valor6
2       Valor7      Valor8      Valor9
3       Valor10     Valor11     Valor12
4       Valor13     Valor14     Valor15
Archivo markdown
Función leer_carpeta(carpeta)

Descripción:

La función leer_carpeta(carpeta) lee todos los archivos .txt en una carpeta y los concatena en un solo DataFrame.

Parámetros:

carpeta: La ruta a la carpeta que contiene los archivos .txt.
Retorno:

Un DataFrame que contiene todos los datos de los archivos .txt en la carpeta.

Pasos a paso:

Importar librerías: Se importan las librerías os y pandas.
Recorrer los archivos de la carpeta: Se utiliza la función os.walk() para recorrer la carpeta especificada y obtener una lista de todos los archivos y subcarpetas.
Validar archivos .txt: Se comprueba si cada archivo en la lista tiene la extensión .txt.
Leer archivos .txt: Se utiliza la función open() para abrir cada archivo .txt en modo lectura.
Convertir archivos a DataFrame: Se utiliza la función pd.read_csv() para convertir cada archivo .txt en un DataFrame.
Agregar DataFrame a una lista: Se agrega cada DataFrame a una lista llamada DataFrame.
Concatenar DataFrames: Se utiliza la función pd.concat() para concatenar todos los DataFrames en la lista DataFrame en un solo DataFrame.
Retornar DataFrame: Se retorna el DataFrame final que contiene todos los datos de los archivos .txt en la carpeta.
Función os.walk():

La función os.walk() es una función de la biblioteca os que se utiliza para recorrer una carpeta y sus subcarpetas. La función devuelve un generador que produce una tupla para cada archivo o subcarpeta en la carpeta
