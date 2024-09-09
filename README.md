# BIG DATA y DATOS EN PEQUEÑA ESCALA

### Diferencias entre Big Data y Datos en Pequeña Escala
## Tamaño del Dataset:

#### Datos en Pequeña Escala: 
- Tienen un tamaño que cabe en la memoria RAM de una sola máquina. Generalmente, esto es desde unos pocos megabytes (MB) hasta algunos gigabytes (GB).
#### Big Data: 
- Supera la capacidad de almacenamiento y procesamiento de una sola máquina. Generalmente involucra terabytes (TB) o petabytes (PB) de datos.

## Capacidad de Procesamiento:

#### Datos en Pequeña Escala: 
- Se pueden procesar y analizar con herramientas estándar como Pandas en Python o Excel en una sola computadora.
#### Big Data: 
- Requiere tecnologías especializadas para procesamiento distribuido, como Hadoop o Apache Spark, y a menudo involucra clústeres de servidores o soluciones en la nube.

## Velocidad de Generación:

#### Datos en Pequeña Escala: 
- La tasa de generación de datos es baja o moderada, y el procesamiento puede realizarse en tiempo no real.
#### Big Data: 
- Los datos se generan a alta velocidad y requieren procesamiento en tiempo real o casi en tiempo real.

## Complejidad de Datos:

#### Datos en Pequeña Escala: 
- Los datos suelen tener una estructura simple y fácil de manejar, como tablas con un número limitado de filas y columnas.
#### Big Data: 
- Los datos pueden ser complejos y variados, incluyendo datos no estructurados (imágenes, textos, videos) y estructuras de datos con alta dimensionalidad.

## Requerimientos de Infraestructura:

#### Datos en Pequeña Escala: 
- Puede utilizar almacenamiento local y computación en una sola máquina o en una red pequeña.
#### Big Data: 
- Necesita infraestructura distribuida para almacenamiento y procesamiento, como sistemas de archivos distribuidos y plataformas en la nube.

## Ejemplos
#### Datos en Pequeña Escala: 
- Un archivo CSV de 100,000 filas que se puede analizar en una laptop.
#### Big Data: 
-  Un dataset de 100 TB de registros de transacciones que se procesa en un clúster de servidores utilizando Apache Spark.

# COMO DESCARGAR PANDAS EN PYTHON

## Asegúrate de tener Python instalado: Primero, verifica si tienes Python instalado. Puedes hacer esto abriendo una ventana de comandos (cmd) y escribiendo:


- Copiar código
~~~
python --version
~~~

### Si Python está instalado, debería mostrar la versión. Si no, descárgalo e instálalo desde python.org.

- Instala pip si no está instalado: pip es el administrador de paquetes para Python. Generalmente, pip se instala automáticamente con Python. Puedes verificar su presencia escribiendo:

- Copiar código
~~~
pip --version
~~~

- Si pip no está instalado, puedes instalarlo siguiendo las instrucciones en la documentación oficial de Python.

### Instala pandas usando pip: Abre una ventana de comandos y escribe:

- Copiar código
~~~
pip install pandas
~~~

### Esto descargará e instalará la biblioteca pandas y sus dependencias.

## Verifica la instalación: Para asegurarte de que pandas se instaló correctamente, abre una consola de Python (escribiendo python en la ventana de comandos) y prueba:
~~~
python
~~~

- Copiar código
~~~
import pandas as pd
print(pd.__version__)
~~~
Esto debería imprimir la versión de pandas que instalaste, confirmando que la instalación fue exitosa.

# ACTIVIDAD

 - Mostrar ultimas 10 filas del dataframe
 - Mostrar informacion del dataframe
 - Obtener valores estadisticos del dataframe
 - Obtener el tamaño del dataframe
 - Seleccionar una columna con [] (forma preferida de seleccionar una columna)
 - Seleccionar 2 columnas usando [[]]

## RESPUESTAS EN FORMATO CODIGO:
- 1:
~~~
import pandas as pd

df = pd.read_csv('historico-nombres.csv')

# Mostrar las últimas 10 filas
print(df.tail(10))
~~~

- 2:
~~~
import pandas as pd

df = pd.read_csv('historico-nombres.csv')

# Mostrar información general del DataFrame
print(df.info())
~~~

- 3:
~~~
import pandas as pd

df = pd.read_csv('historico-nombres.csv')

# Obtener estadísticas descriptivas del DataFrame
print(df.describe())
~~~

- 4:
~~~
import pandas as pd

df = pd.read_csv('historico-nombres.csv')

# Obtener el tamaño del DataFrame (filas, columnas)
print(df.shape)
~~~

- 5:
~~~
import pandas as pd

df = pd.read_csv('historico-nombres.csv')

# Seleccionar una columna usando []
# Supongamos que la columna se llama 'nombre'
print(df['nombre'])
~~~

- 6:
~~~
import pandas as pd

df = pd.read_csv('historico-nombres.csv')

# Seleccionar dos columnas usando [ [] ]
# Supongamos que las columnas se llaman 'nombre' y 'año'
print(df[['nombre', 'anio']])
~~~


