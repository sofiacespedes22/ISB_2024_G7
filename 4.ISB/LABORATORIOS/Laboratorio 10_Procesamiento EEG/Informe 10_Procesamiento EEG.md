# Laboratorio N°10 - Procesamiento de señales EEG
## **Tabla de contenidos**
1. [Introducción](#introduccion)\
   1.1 [Marco teórico](#marco)
2. [Objetivos](#objetivos)
3. [Metodología](#metodologia)\
   3.1 [Materiales y equipos](#materiales)\
   3.2 [Procedimiento](#adquisicion)
4. [Resultados](#resultados)
5. [Archivos](#archivos)
6. [Discusión](#discusion)
7. [Referencias bibliográficas](#referencias)

<a name="introduccion"></a>
## **INTRODUCIÓN**
### **CONTEXTO**


<a name="marco"></a>
### **MARCO TEÓRICO**


## OBJETIVOS
* Investigar literatura científica sobre técnica de procesamiento de señales electroencefalográficas (EEG).
* Identificar e implementar la mejor técnica filtrado para eliminar el ruido de las señales EEG.

<a name="metodologia"></a>
## METODOLOGÍA 
Para este laboratorio, se utilizarán la base de datos Physionet para 

<a name="materiales"></a>
### 1. MATERIALES Y EQUIPOS

<div align="center">

|  **Modelo**  | **Descripción** | **Cantidad** | **Imagen** |
|:------------:|:---------------:|:------------:|:----------:|
|-|**Laptop o PC**: Laptop equipada con el programa Python, para poder implementar ahí el código, para realizar los respectivos filtrados|1|<image width="300" height="100" src="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/1e850abc-e826-47a5-aa7b-292a134d94ec">|

<p align="center"><i>Tabla 1. Materiales y equipos utilizados</i></p>
</div>

<a name="adquisicion"></a>
### 2. PROCEDIMIENTO
Para el procedimiento del procesamiento de las señales EEG, se utilizó un artículo de referencia el cual presenta un análisis de las señales EEG para el diagnóstico de desórdenes neurológicos utilizando la transformada wavelet (DWT) y técnicas de filtrado y clasificación [x]. Las señales fueron previamente pre-procesadas mediante el uso de filtros, sus características fueron extraídas y se utilizaron técnicas de clasificación de vectores. Se combinaron técnicas dentro de la extracción de características como la banda de potencia logarítmica, desviación estándar, varianza, kurtosis y entropía de Shannon, utilizando clasificadores de diferentes tipos. Se presenta, a continuación, un diagrama de bloques que ejemplifica el procesamiento de las señales basadas en DWT.

</div>
<p align="center">
<image width="300" height="150" src="[https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/736e7588-584e-4b8d-bce9-751c3284a120](https://github.com/sofiacespedes22/ISB_2024_G8/assets/164461832/94395227-58c9-49f7-ade4-45aa67303d9f)">
<p align="center"><i>Figura x. Diagrama de bloques del procedimiento a seguir basado en la literatura [x] </i></p>
</div>


#### Pre-procesamiento
Para el pre-procesamiento de la señal que presentaba artefactos, ruidos e interferencias de diversas fuentes, se aplicó la técnica ICA y filtros adaptativos para eliminar para eliminar los artefactos oculares de las señales registradas. Posteriormente, las señales fueron segmentadas en ventanas de tiempo de 50 s. Luego de la segmentación, se aplicó un filtrado pasa banda, que incluyo filtros FIR e IIR (Chebyshev, Butterworth).

#### Extracción de características
Para la extracción de características, se utilizó la DWT basado en LBP, desviación estándar, varianza, kurtosis y entropía para formar los vectores de características, que se observan en la Tabla 2. La DWT fue empleada debido a que proporciona una representación wavelet altamente eficiente. Se empleó la familia Daubechies 4 (db4) como la función wavelet madre de nivel 4. En la descomposición de primer nivel, se utilizó filtros paso-bajo y paso-alto para obtener la representación de la señal digital como coeficientes de aproximación (A1) y detalle (D1). Los coeficientes de aproximación y detalle en cada nivel fueron seleccionados después de obtener todos los coeficientes de detalle en cada nivel (D1, D2, D3 y D4) y los coeficientes de aproximación en el último nivel (A4).



</div>
<p align="center">
<image width="300" height="150" src="[https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/736e7588-584e-4b8d-bce9-751c3284a120](https://github.com/sofiacespedes22/ISB_2024_G8/assets/164461832/94395227-58c9-49f7-ade4-45aa67303d9f)">
<p align="center"><i>Figura x. Diagrama de bloques del procedimiento a seguir basado en la literatura [x] </i></p>
</div>


#### Clasificación
Por último, para la clasificación, se emplearon como clasificadores las técnicas de análisis discriminante lineal LDA, SVM, KNN y ANN. Durante el proceso de entrenamiento del algoritmo, los vectores de características se aplican a la red para ajustar sus parámetros variables, pesos y sesgos.

<a name="resultados"></a>
## RESULTADOS
### Estado de reposo


### Estado de respiración prolongada


### Estado de ejercicio intensivo


<a name="archivos"></a>
## ARCHIVO DE LA SEÑAL PLOTEADA EN PYTHON
* **Codigo**
  - []()

<a name="discusion"></a>
## Discusión

<a name="conclusion"></a>
## Conclusión


<a name="referencias"></a>
## REFERENCIAS BIBLIOGRÁFICAS