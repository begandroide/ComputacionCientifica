# Tarea 3 - Computación científica

Tarea respectiva a interpolación de videos, aplicando _Motion-Compensated Frame interpolation_. Con el objetivo de aumentar el _frame-rate_ de un video, mejorando la calidad y fluidez de un video.

## Consideraciones
El notebook viene con los resultados de todas las secciones requeridas en las carpetas **./Results/\*** y en **./Comparisions/\***. 
Se recomienda utilizar estos para ver como se comporta el error (sección 2) o para concatenar videos. 

Por otro lado, se recomienda correr notebook en un computador con sistema operativo distinto a _windows_, ya que este presenta problemas y mal manejo de memoría. En Linux no hay problemas con memoría, debido a la utilización de la partición Swap.

## Autor

* **Benjamín Gautier Ortiz** - *201460036-4* - **benjamin.gautier.14@sansano.usm.cl** 

## Librerías utilizadas

* Numpy
* Imutils
* Cv2 > para leer los videos como un stream.
* Matplotlib.pyplot > para graficar resultados.
* scipy.interpolate > biblioteca con distintos métodos interpoladores a ser utilizados.
* base64
* IPython.display
* Ipywidgets > widget para hacer la visualización de resultados interactiva.
* os
* %time > Comando mágico de jupyter notebook que mide el wall-time y Cpu-time.
  
**Arreglar el scipy.interpolate**

Método | Distrib. puntos | 5->15 | 5->60 | 15->30 | 30->60
---------|:----------:|:---------: |:---------:|:---------:|---------:
 Spline-lineal   | Equi | 20.2s     | 24.6s| 24s  | 27.2s
 Spline-lineal   | Cheb | 20.3s     | 24.4s| 24.2s| 26.1s
 Spline-cubica | Equi | 43.1s     | 44.3s| 47.3s| 48.1s
 Spline-cubica | Cheb | 42.7s    | 45.3s| 45.9s| 48.1s
 Baricéntrica   | Equi | 1m 12s | 1m 26s| 5m 53s| 11m 10s
 Baricéntrica   | Cheb | 1m 14s | 1m 26s| 6, 5s| 10m 59s