# Laboratorio N°5 - Procedimiento de registro de señales de electroencefalograma (EEG)
## **Tabla de contenidos**
1. [Lista de participantes](#lista)
2. [Introducción](#introduccion)\
   2.1 [Contexto](#contexto)\
   2.2 [Marco teórico](#marco)
3. [Objetivos](#objetivos)
4. [Metodología](#metodologia)\
   4.1 [Materiales y equipos](#materiales)\
   4.2 [Procedimiento](#adquisicion)\
   4.3 [Procesamiento de datos](#procesamiento)
5. [Resultados](#resultados)\
   5.1 [Archivos](#archivos)
6. [Discusión](#discusion)
7. [Conclusiones](#conclusiones)
8. [Referencias bibliográficas](#referencias)


<a name="lista"></a>
## **Lista de participantes**
- Sofia Camila Céspedes Trece - 71738148
- Nicole Stefany Acuña Malpartida - 71400976
- Chris Margory Viviano Salvatierra - 75138288
- Harold Alonso Alemán Ramírez - 71386429
  
<a name="introduccion"></a>
## **Introducción**
<a name="contexto"></a>
### **Contexto**
#### **a. Encefalografía**
Un electroencefalograma (EEG) es una téncica no invasiva usada en el ámbito de la neurología, el cual sirve para medir las diferentes señales eléctricas creadas por la actividad de grandes grupos de neuronas, durante un determinado periodo de tiempo, a través de electrodos <sup>[1](https://www.mdpi.com/2076-3417/10/21/7453)</sup>. La neuronas cerebrales establecen comunicación a través de impulsos eléctricos, incluso cuando estamos dormidos. Y esta actividad es la que el electroencefalográgico registra como líneas onduladas <sup>[2](https://www.mayoclinic.org/es/tests-procedures/eeg/about/pac-20393875)</sup> .El electroencefalograma funciona midiendo las fluctuaciones de la corriente eléctrica entre la piel y el sensor, en este caso de los electrodos, amplicando la corriente eléctrica y realizando filtrado de ser necesario <sup>[1](https://www.mdpi.com/2076-3417/10/21/7453)</sup>.

</div>
<p align="center">
<image width="500" height="350"src="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/b74e6a58-fd60-4514-96f0-81cc09cd571d">
<p align="center"><i>Figura 1. Actividad cerebral registrada por encefalograma <sup>[2](https://www.mayoclinic.org/es/tests-procedures/eeg/about/pac-20393875)</sup> </i></p>
</div>


#### **b. Patologías que pueden ser detectadas con EEG**<sup> [1](https://www.mdpi.com/2076-3417/10/21/7453)</sup>
Este procedimiento no invasivo es útil, ya que los resultados que arrojan nos permiten visualizar cambios en la actividad cerebral, los cuales luego de ser interpretados nos proporcionan información, que nos ayuda a diagnosticar y predecir muchas enfermedades cerebrales anormales y deterioros cognitivos. A continuación se mencionarán solo algunas de las enfermedades que pueden ser diagnosticadas:
1. Epilepsia
2. Enfermedad de Parkinson
3. Problemas de memoria como el Alzheimer
4. Deficiencias del lenguaje como dislexia
5. Trastorno por déficit de atención e hiperactividad (TDHA)
6. Convulsiones
7. Esquizofrenia
8. Autismo en adultos y niños 
9. Trastornos del sueño e insomnio, ansiedad , estrés
10. Tumores cerebrales
11. Encefalitis herpética
12. Accidente cerebrovascular

#### **c. Aplicaciones** <sup> [1](https://www.mdpi.com/2076-3417/10/21/7453)</sup>
Los dispositivos EEG pueden proporcionar información valiosa sobre el estado de salud mental de las personas, y contribuir también a la investigación. Entre algunas de las aplicaciones del EEG podemos encontrar:\
* **Interfaces cerebro-computadora (BCI)** : El BCI es una de las aplicaciones comunes del EEG, en donde utilizan los datos obtenidos del EEG en tiempo real, para controlar dispositivos mecánicos y electrónicos. El BCI principlamente se puede usar en 3 ámbitos:
1. Navegación autónoma de dispoditivos digitales, con orientación a la teleoperación en tiempo real de cuerpos robóticos y monitoreo de sensores.
2. Como ayuda para personas con discapacidades motoras leves, con el fin de facilitarles sus actividades,  
Entre otro de lcomo en el control de aplicaciones móviles, dirigir movimientos de sillas de ruedas eléctricas, sistemas de reconocimiento de voz para personas con discapacidad de habla, etc.
3. Neurojuegos y entretenimiento.   

* **Investigación en neurociencia** :
Para comprender la funcionalidad del sistema nervioso, el EEG es usado como herramienta para aprender sobre el funcionamiento del cerebro cuando experimenta diferentes estados emocionales y como funciona el cerebro en diversos estados mentales. Algunos de los campos en los que se realiza comunmente investigacionesson en:
1. Neurociencia cognitiva
2. Neurociencia conductual
3. Neurofisiología


<a name="marco"></a>
### Marco teórico

#### **a. ¿Qué es una señal EEG?**
<p align="justify">
El electroencefalograma (EEG) es una técnica de neuroimagen no invasiva que permite el registro de la actividad eléctrica del cerebro mediante la colocación de electrodos en el cuero cabelludo que detectan la señal <sup>[3](https://www.frontiersin.org/articles/10.3389/fncom.2023.1151852/full)</sup> . Estas señales brindan información en cuanto a los diferentes mecanismos operativos que presenta el cerebro, permitiendo la identificación de patrones, trastornos neurológicos y explorar diversos procesos cognitivos como la memoria, atención o percepción<sup>[4](https://www.sciencedirect.com/science/article/pii/S092549272300001X)</sup> . Asimismo, el EEG representa un patrón de señal que es obtenida amplificando y registrando el potencial biológico del cerebro en el cuero cabelludo. Este potencial refleja la actividad macroscópica de la superficie cerebral y permite que los electrodos capturen los impulsos eléctricos inherentes y periódicos generados por grupos de células cerebrales <sup>[5](https://www.mdpi.com/1424-8220/23/14/6434)</sup>. Las oscilaciones e voltaje que presentan estas señales revelan cierta actividad cerebral significativa, lo cual se refleja en estados de sueño profundo o en coma, donde las oscilaciones son lentas y las amplitudes elevadas<sup>[6]()</sup>. 
 </p>


</div>
<p align="center">
<image width="500" height="350"src="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164461832/1971c8a3-8cf5-4ce0-a9d1-e974308ce70f">
<p align="center"><i>Figura 2.  <sup>[2](https://www.mayoclinic.org/es/tests-procedures/eeg/about/pac-20393875)</sup> </i></p>
</div>


#### b. Oscilaciones del EEG
<p align="justify">
Para la interpretación del EEG, es importante considerar la caracterización que presentan las señales en función a su ubicación, amplitud, frecuencia, morfología, continuidad, simetría o reactividad. Sin embargo, el método más utilizado para interpretar es a partir de la frecuencia, estipulando que la señal medida es una mezcla de diferentes frecuencias subyacentes que se consideran reflejo de estados cognitivios, afectivos o de atención. A continuación, se observa una tabla de la clasificación de las ondas cerebrales según la frecuencia<sup>[7] (https://doi.org/10.1016/j.ijpsycho.2015.02.003)</sup> <sup>[8](https://www.ncbi.nlm.nih.gov/books/NBK539805/)</sup>:
</p>
<div align="center">
	
|  **Tipo de banda**  | **Frecuencia (Hz)** | **Estado del cerebro** |
|:------------:|:---------------:|:------------:|
|Delta|0.5 - 4.0|<p align="justify"> La banda delta es la oscilación más lenta y de mayor amplitud del EEG. Aparece durante el sueño profundo y contribuye a la consolidación de la memoria y el aprendizaje. Normalmente, se observa en las regiones frontocentrales de la cabeza, pero su presencia en estados de vigilia puede indicar problemas cerebrales como encefalopatía o disfunción focal.</p>|
|Theta|4.0 - 7.0|<p align="justify"> La banda theta del EEG está relacionada con la somnolencia y las etapas iniciales del sueño, predominando en las regiones frontocentrales y reemplazando al ritmo alfa con el aumento de la somnolencia. Además, se intensifica durante emociones fuertes y en tareas mentales desafiantes. Su presencia focal en la vigilia puede indicar disfunción cerebral focal y está asociada con la atención y la memoria de trabajo.</p>|
|Alpha|8.0 - 12.0|<p align="justify"> El ritmo alfa dominante posterior se observa en EEG normales de personas despiertas, ubicado en la región occipital. Es el ritmo de fondo de EEG en adultos y suele mantenerse estable desde los 3 años hasta la novena década de vida en individuos sanos. Variaciones rápidas de este ritmo pueden ocurrir en personas normales. Su ralentización sugiere disfunción cerebral generalizada. El ritmo alfa está relacionado con la relajación y la inhibición sensorial, aumentando con los ojos cerrados y relajación, y disminuyendo con actividad y ojos abiertos.</p>|
|Beta|13.0 - 30.0|<p align="justify"> El ritmo beta es el ritmo EEG más común en adultos y niños normales. Predomina en las regiones frontal y central de la cabeza y se debilita hacia las áreas posteriores. Se relaciona con el pensamiento activo, la concentración y la planificación de movimientos. También puede activarse cuando se observan movimientos de otras personas.</p>|
|Gamma|>30|<p align="justify"> El ritmo gamma pertenece a la clasificación de ondas de alta frecuencia. Su importancia en diversas funciones cognitivas está bien documentada. Estos ritmos pueden ser útiles para detectar desmielinización y otros problemas de integridad cortical. Se sugiere que los ritmos gamma están relacionados con la integración de percepciones sensoriales y la atención.</p>|
<p align="center"><i>Tabla 1. Materiales y equipos </i></p>
</div>


#### c. Activación neural
El cerebro se compone de millones de neuronas interconectadas que generan potenciales eléctricos. Como se mencionó previamente, esta actividad es detectada a partir del EEG, utilizando electrodos que registran los dipolos eléctricos creados por poblaciones neuronales situadas perpendicularmente a la superficie de la cabeza, principalmente por neuronas piramidales ubicadas entre las capas 3 y 5 de la corteza cerebral. Estas neuronas generan campos eléctricos como resultado de señales electroquímicas transmitidas entre ellas. Cuando generan campos eléctricos al mismo tiempo, estos son lo suficientemente significativos para ser captados por el EEG <sup> [9](https://doi.org/10.1016/j.tins.2017.02.004)</sup> .Asimismo, a nivel fisiológico, las señales del EEG provienen de las corrientes iónicas transmembrana en las neuronas piramidales; estas células, se encuentran en todas las áreas de la corteza cerebral: occipital, temporal, parietal y frontal, y están siempre orientadas perpendicularmente a la superficie cortical, con el cuerpo celular dirigido hacia el interior del cerebro y las dendritas apuntando hacia la superficie cortical <sup> [10](https://onlinelibrary.wiley.com/doi/full/10.1684/epd.2020.1217)</sup> .



#### d. Artefactos
Si bien el EEG permite registrar la actividad eléctrica cerebral, también registra actividades eléctricas que se originan en lugares distintos del cerebro. Esta actividad registrada se denomina artefacto pues no es de origen cerebral y puede dificultar la interpretación clínica o el posterior análisis cuantitativo. Los artefactos surgen de fuentes fisiológicas, como ritmo cardíaco, actividad muscular o movimiento ocular y extrafisiológicas, como el ruido ambiental o del propio sistema de medición <sup> [11]()</sup> <sup> [12]()</sup> . Por ello, resulta importante considerar protocolos para la adquisición correcta de las señales EEG que permitan disminuir la mayor cantidad de artefactos y un correcto pre-procesamiento de la señal para su análisis posterior. 

<a name="objetivos"></a>
## Objetivos
1. Adquirir señales biomédicas de EEG.
2. Hacer una correcta configuración de BiTalino y Ultracortex Mark IV.
3. Extraer la información de las señales ECG del software OpenSignals (r)evolution y OpenBCI
   
<a name="metodologia"></a>
## Metodología 
La metodología seguida para la adquisición y procesamiento de las señales EEG utilizando el kit BITalino fue implementada siguiendo el protocolo de adquisición y posicionamiento de los electrodos de la guía “"BITalino HOME-GUIDE #3 ELECTROENCEFALOGRAM(ECG) Exploring Signals at the Skin Surface"<sup> [11](https://support.pluxbiosignals.com/wp-content/uploads/2022/04/HomeGuide3_EEG.pdf)</sup>. Asimismo, se utilizó el Ultracortex Mark IV EEG Headset siguiendo el sistema 10-20 [ref2], que es el estándar aceptado internacionalmente para la colocación de electrodos en el contexto del EEG.

<a name="materiales"></a>
### 1. Materiales y Equipos
<div align="center">
	
|  **Modelo**  | **Descripción** | **Cantidad** | **Imagen** |
|:------------:|:---------------:|:------------:|:----------:|
|(R)EVOLUTION|**Kit BITalino**:Kit electrónico formada por varios módulos individuales utilizados para la recolección de datos boiomédicos. Se pueden adquirir señales como EMG,ECG o EEG.|1|<image src="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/c8d4e3ed-4054-4c4d-9820-0c1dbd5ddd6f">|
|-|**Laptop o PC**:Se descargará el software de análisis para procesar las señales|1|<image width="300" height="200" src="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/1e850abc-e826-47a5-aa7b-292a134d94ec">|
|-|**Electrodos**: Registran la actividad eléctrica de los músculos durante la contracción y relajamiento muscular|3|<image width="300" height="200" src="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/21dab0fa-801d-4dd1-b0c9-3b29bf3be7fb">|
|OpenBCI|**Ultracortex Mark IV EEG Headset** : Es un casco de encefalografía diseñado para registrar actividad eléctrica del cerebro, utilizada comúnmente en investigaciones relacionadas con la neurociencia, la interfaz cerebro-computadora (BCI) y monitorización de la salud mental|1|<image width="300" height="200" src="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/62500fc6-f80b-4aed-88de-dfb30c20a060">|
|OpenBCI|**OpenBCI Cyton 8-channel Board** : Es una placa de adquisición de datos de electroencefalografía (EEG) de ocho canales fabricada por OpenBCI|1|<image width="300" height="200" src="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/8735fad8-29d3-4401-b952-f3df243f17d1">|
<p align="center"><i>Tabla 1. Materiales y equipos </i></p>
</div>



<a name="adquisicion"></a>
### 2. Procedimiento
Para la adquisición de datos, el sujeto de prueba fue una mujer de 22 años con las siguientes características:
<div align="center">
	
|  **Edad**  | **Peso** | **Sexo** | **Condición** |
|:------------:|:---------------:|:------------:|:----------:|
|22|58 kg|Femenino|Sano|
<p align="center"><i>Tabla 2. Características del sujeto de prueba escogido </i></p>
</div>

#### Protocolo de conexión
En primer lugar, se realizó la conexión entre el BITalino con el programa OpenSignal para visualizar la señal generada a partir de Bluetooth. Luego, se realizó la conexion EEG en la placa del BITalino utilizando el sensor EEG de 3 electrodos. Posteriormente, se realizó el posicionamiento de los electrodos en el sujeto de prueba para realizar la configuración bipolares de acuerdo al sistema internacional 10-20. En esta configuración, se colocaron los electrodos de la siguiente manera, también observada en la Tabla 3:
* **FP1** (electrodo positivo/rojo) se coloca en la sección de la frente izquierda .
* **FP2** (electrodo negativo/negro) se coloca en la sección de la frente derecha.
* **REF** (electrodo de referencia/blanco) se coloca en el hueso mastoideo, debido a que representa una zona de baja interferencia electromagnética.


<div align="center">	
	
|  **Colocación de electrodos para el registro de señales EEG con el Kit Bitalino**  | **Colocación de electrodos para el registro de las señales EEG con el Open BCI Ultracortex Mark IV** | 
|:------------:|:--------:|
|<image src="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/7662c920-4066-4869-8268-9ae4a66a83e5">|<image width="450" height="300" src="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/e3011564-1b5d-4230-a901-0898b5af9709">|
<p align="center"><i>Tabla 3. Posicionamiento de los electrodos en el sujeto de prueba</i></p>
</div>

#### Protocolo de adquisición
Para la adquisición de datos, se realizó el protocolo de adquisición brindado por la guía y los docentes del curso en la cual se registraron las señales EEG para el análisis en cuatro diferentes estados:

**a. Estado de reposo**: El sujeto de prueba se quedó en una posición estable y manteniendo la calma para el registro de una línea base de señal con poco ruido y sin movimientos. Este estado representa nuestra prueba control. El registro de la señal fue grabado por 30 segundos.

**b. Estado de ojos cerrado-ojos abiertos**: El sujeto mantuvo los ojos cerrados y abiertos completando un ciclo (5 veces cada estado), manteniendo ambas fases durante 5 segundos. Para evitar artefactos, el sujeto se mantuvo calmado y mirando hacia un punto específico. El registro de la señal fue grabado por 50 segundos.

**c. Estado de segundo reposo**: Tras la primera actividad, el sujeto de prueba mantuvo nuevamente el estado de calma y sin movimiento como segunda fase de referencia. El registro de la señal fue grabado por 30 segundos.

**d. Estado de preguntas**: Se realizaron una serie de ejercicios matemáticos [ref3] de menor a mayor complejidad al sujeto de prueba para que pueda resolverlo mentalmente enfocando su mirada en un punto específicos para evitar artefactos. La duración entre el lapso de registro de la respuesta y la siguiente pregunta fue de 12 segundos. Las preguntas realizadas se observan en la Tabla 4.

|  **Categoría**  | **Pregunta** | 
|:------------:|:---------------:|
|**Simple**|<p align="justify"> Hay 3 pájaros en un árbol; Llegan 7 más. ¿Cuántos pájaros hay ahora?</p>|
|**Simple**|<p align="justify"> Jonás tiene 5 manzanas y Mary tiene 4. ¿Cuántas manzanas tienen en total?</p>|
|**Simple**|<p align="justify"> Hanna tiene 9 dólares pero gastó 4. ¿Cuántos dólares le quedan?</p>|
|**Compleja**|<p align="justify"> John anotó 45 puntos para su equipo; 10 más que José. Marie anotó 13 puntos más que John y Joseph juntos. ¿Cuántos puntos obtuvieron en total?</p>|
|**Compleja**|<p align="justify"> El grupo A tiene 24 estudiantes; 13 menos que el grupo B. El grupo C tiene 12 alumnos más que los grupos A y B juntos. ¿Cuál es el número total de estudiantes?</p>|
|**Compleja**|<p align="justify"> Una tienda vendió 21 refrescos por la mañana y 13 más que por la tarde. Por la noche vendió 10 más que por la mañana y por la tarde juntas. ¿Cuántos refrescos se vendieron en total?</p>|
<p align="center"><i>Tabla 4. Preguntas realizadas al sujeto de prueba </i></p>
</div>

<a name="procesamiento"></a>
### 3. Procesamiento de datos
Para el procesamiento de las señales adquiridas, se realizó el ploteo en Python para el análisis cuantitativo de segmentos específicos y determinar las características de cada señal EEG, así como los intervalos de duración de cada parámetro. Asimismo, se realizó la transformada rápida de Fourier (FFT) para determinar las frecuencias.

<a name="resultados"></a>
## Resultados
<a name="videos"></a>
###  Visualización de señal eléctrica mediante video y OpenSignals
A continuación se pueden observar los videos correspondientes, tanto del sujeto de prueba como de la señals señales:
<div align="center">	
	
| **Estados** | **Videos** |
|:------------:|:---------------:|
| **a. Estado de reposo**|<video width="300" height="200" src="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/60a9c0ed-fcfd-4c2f-9139-7b9dd845d8f8">|
| **b. Estado de ojos cerrado-ojos abiertos**|<video width="300" height="200" src="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/8cc12b02-0daf-4a6d-9831-6299945492e2">|
| **c. Estado de segundo reposo**|<video width="300" height="200" src="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/5aba84d2-9a56-4b4f-a673-329ed3819a50">|
| **d. Estado de preguntas**|<video width="300" height="200" src="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/959c0340-0668-4424-9f28-764e0b352842">|


<a name="archivos"></a>
### Archivo de las señales ploteadas en Python
   
<a name="discusion"></a>
## Discusión

<a name="conclusiones"></a>
## Conclusiones

<a name="referencias"></a>
## Referencias bibliográficas
[1] https://www.mdpi.com/2076-3417/10/21/7453
[2] https://www.mayoclinic.org/es/tests-procedures/eeg/about/pac-20393875
[3] Islam M.K., Rastegarnia A. Recent advances in EEG (non-invasive) based BCI applications. Front. Comput. Neurosci. 2023;17:1151852. doi: 10.3389/fncom.2023.1151852.
[4] Patil A.U., Lin C., Lee S.H., Huang H.W., Wu S.C., Madathil D., Huang C.M. Review of EEG-based neurofeedback as a therapeutic intervention to treat depression. Psychiatry Res. Neuroimaging. 2023;329:111591. doi: 10.1016/j.pscychresns.2023.111591.
[5] Chaddad, A., Wu, Y., Kateb, R., & Bouridane, A. (2023). Electroencephalography Signal Processing: A Comprehensive Review and Analysis of Methods and Techniques. Sensors (Basel, Switzerland), 23(14), 6434. https://doi.org/10.3390/s23146434
[6] B. Giesbrecht and J. Garrett, "Electroencephalography," Reference Module in Neuroscience and Biobehavioral Psychology, Jan. 2024, doi: 10.1016/B978-0-12-820480-1.00007-3.
[7] Herrmann, C. S., Strüber, D., Helfrich, R. F., & Engel, A. K. (2016). EEG oscillations: From correlation to causality. International journal of psychophysiology: official journal of the International Organization of Psychophysiology, 103, 12–21. https://doi.org/10.1016/j.ijpsycho.2015.02.003
[8] Nayak CS, Anilkumar AC. EEG Normal Waveforms. [Updated 2023 Jul 24]. In: StatPearls [Internet]. Treasure Island (FL): StatPearls Publishing; 2024 Jan-. Available from: https://www.ncbi.nlm.nih.gov/books/NBK539805/
[9] Cohen, M. X. (2017). Where does EEG come from  and  what  does  it  mean? Trends  in Neurosciences, 40(4), 208-218.https://doi.org/10.1016/j.tins.2017.02.004
[10] S. Beniczky and D. L. Schomer, "Electroencephalography: basic biophysical and technological aspects important for clinical applications," Epileptic Disorders, vol. 22, no. 6, pp. 697–715, Dec. 2020, doi: 10.1684/EPD.2020.1217.
[11] Urigüen JA, Garcia-Zapirain B. EEG artifact removal-state-of-the-art and guidelines. J Neural Eng. 2015 Jun. 12 (3):031001.
[12] Zhang C, Tong L, Zeng Y, Jiang J, Bu H, Yan B, et al. Automatic Artifact Removal from Electroencephalogram Data Based on A Priori Artifact Information. Biomed Res Int. 2015. 2015:720450.
