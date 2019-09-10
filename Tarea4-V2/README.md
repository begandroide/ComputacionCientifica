# Tarea 4 - Computación científica

Tarea respectiva a resolver sistemas de ecuaciones sobredeterminados, aplicando _método extendido de newton_. Con el objetivo de dar las soluciones de un sistema que no tiene solución mediante análisis numérico.

## Consideraciones

Se han dejado los parámetros ideales para correr cada algoritmo y tener tiempos razonables de revisión ( menor a 5 minutos por pregunta). 

Por otro lado, se recomienda correr notebook en un computador con sistema operativo distinto a _windows_, ya que este presenta problemas y mal manejo de memoría. En Linux no hay problemas con memoría, debido a la utilización de la partición Swap.


## Autor

* **Benjamín Gautier Ortiz** - *201460036-4* - **benjamin.gautier.14@sansano.usm.cl** 

## Librerías utilizadas

* Numpy > Numeric Python, para manejo de vectores, matrices y operaciones relacionadas.
* scipy.lu > para realizar la descomposición PA=LU
* scipy.sparse.csr_matriz > para utilizar estructura de datos para matrices sparse.
* scipy.sparse.identity > para usar matrices identidades de tipo sparse.
* scipy.solve_triangular > para resolver sistemas lineales triangulares.
* scipy.sparse.linalg.gmres > para resolver sistemas de ec. lineales mediante GMRes.
* Matplotlib.pyplot > para graficar resultados.
* Ipywidgets > widget para hacer la visualización de resultados interactiva.
* timeit > librería para registrar tiempos de cómputo de las distintas secciones.
* %time > Comando mágico de jupyter notebook que mide el wall-time y Cpu-time.
