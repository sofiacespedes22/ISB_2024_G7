# LABORATORIO N°2 - ADQUISICIÓN DE SEÑALES Y GRAFICACIÓN EN ARDUINO
## Tabla de contenidos
1. [Lista de participantes](#lista)
2. [Objetivos](#objetivos)
3. [Materiales y Equipos](#materiales)
4. [Entregables](#entregables)
5. [Metodología](#metodologia)
   - [Configuración inicial de los equipos](#conec1)
   - [Conexión del arduino nano 33 IoT](#conec2)
6. [Resultados y discusión](#resultados)
   - [Señal sinusoidal](#sinusoidal)
   - [Señal cuadrada](#cuadrada)
   - [Señal rampa](#rampa)
   - [Señal pulso](#pulso)
   - [Fuentes de error](#error)
7. [Referencias bibliográficas](#referencias)

<a name="lista"></a>
## Lista de participantes
- Sofia Camila Céspedes Trece - 71738148
- Nicole Stefany Acuña Malpartida - 71400976
- Chris Margory Viviano Salvatierra - 75138288
- Harold Alonso Alemán Ramírez - 71386429
  
<a name="objetivos"></a>
## Objetivos
1. Adquirir señales conocidas como señal cuadrada, triangular, senoidal, rampa, etc.
2. Entender los criterios de selección de la frecuencia de muestreo.
3. Manipular y configurar adecuadamente una fuente de alimentación regulable; multímetro digital; Generador de señales y osciloscopio digital.
   
<a name="materiales"></a>
## Materiales y Equipos
<div align="center">
   
|  **Modelo**  | **Descripción** | **Cantidad** | **Imagen** |
|:------------:|:---------------:|:------------:|:----------:|
| AFG1022 | Generador de señales | 1 | <image width="200" height="150" src="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/f77e565c-b14c-4dd4-9bf5-9d63af9b054d"> | 
 | TBS 1000C Series | Osciloscopio digital | 1 | <image width="200" height="150" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/d422cbc6-285c-483d-ab3b-eb10b246ac21"> 
| SAMD | Arduino 33 IoT | 1 | <image width="200" height="150" src="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/9bb89063-e51a-4ef1-9764-a4d6ffc2710a"> |
| - | Cable BNC M-M | 1 | <image width="200" height="150" src="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/1030c4cf-863e-4986-9043-51f2ef09e90b"> |
| - | Punta de osciloscopio con conector BNC (Male) | 1 | <image width="200" height="150" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/dd841cab-94c3-40ba-b2f6-3f165949aa44"> |
| - | Par de cables M-M | 1 | <image width="200" height="150" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/ba69efad-205a-4ae4-a563-0e8fd357f851"> |
| - | Condensador | 1 | <image width="200" height="150" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/2648872d-9dde-41ce-a7b8-81f828d5d3e6"> |
| - | Protoboard | 1 | <image width="200" height="150" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/8a071497-cdd1-4dbc-bbfc-a00e4cfc48b5">

</div>
<p align="center"><i>Tabla 1. Materiales y equipos utilizados para el ploteo de señales</i></p>

<a name="entregables"></a>
## Entregables
- Plotear al menos 3 señales en Arduino IDE provenientes del generador de señales.
- Comparar las señales graficadas del Arduino IDE con las gráficas obtenidas del osciloscopio.
- Graficar en Arduino cloud.

<a name="metodologia"></a>
## Metodología
<a name="conec1"></a>
### Configuración inicial de los equipos
<div align="justify">

Antes de comenzar con la práctica de laboratorio, se configuró el generador de señales y el osciloscopio. El generador de señales fue configurado inicialmente para proporcionar una señal sinusoidal de 1 kHz de frecuencia, con 3V de amplitud y 0V de offset. Tras la configuración, se conectó el cable BNC entre los puertos del canal 1 tanto del generador de ondas como del osciloscopio, como se observa en la Figura 1.

<p align="center">  
<image width="500" height="350" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/0561535c-8e5e-4988-8c1d-482a538f316a"> 
</p>
<p align="center"><i>Figura 1. Configuración del generador de ondas para el ploteo de señales</i></p>

<div align="justify">
  
A partir del uso de los cursores y controles de posición vertical, horizontal y disparo se ajustó la visualización de la señal sinusoidal, considerando la escala en la que se encontraba la sonda. Se mostró las medidas de amplitud y periodo de la señal con el uso de estos cursores, como se observa en la Figura 2.

</div>
<p align="center">   
<image width="500" height="350" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/2a873926-4777-4f71-a4b3-c66556a9b1cf">
</p>
<p align="center"><i>Figura 2. Señal sinusoidal visualizada en el osciloscopio para el ploteo de señales</i></p>
<a name="conec2"></a>
   
### Conexión del arduino nano 33 IoT 
<div align="justify">
Se realizó la conexión del Arduino nano 33 IoT conectado al protoboard junto a un condensador formando un filtro RC con el cable BNC para evaluar la señal sinusoidal enviada desde el generador de señales, observado en la Figura 3. 
   
<p align="center"> 
<image width="500" height="350" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/3f0490da-5c96-4ae8-99a6-f0bac5c4c7b2">
</p>
<p align="center"><i>Figura 3. Conexión Arduino nano 33 IoT y cable BNC para el ploteo de señales</i></p>
<div align="justify">
De manera paralela, se modificó el código en Arduino SAMD adjuntado por los docentes para que permita leer el puerto por el cual esta conectado al generador y la visualización de la gráfica generada. El código modificado se encuentra adjuntado en la carpeta “Código”. A continuación, se visualiza los parámetros considerados para el ploteo de las señales que se compararán en la siguiente sección (ver Tabla 2).
</div>
<div align="center">

| Parámetros | Valor | 
| ------------ | ------------ | 
| Frecuencia        | 3 hz    | 
| Voltaje    | 1.5 V    | 
| Offset    | 0 V   | 
| Capacitor    | 100 µF  | 

</div>
<p align="center"><i>Tabla 2. Parámetros considerados para el ploteo de señales</i></p>

<a name="resultados"></a>
## Resultados y discusión
<div align="justify">
En el presente informe, se generaron diferentes tipos de señales (sinusoidal, cuadrada, rampa y pulso) considerando los parámetros de frecuencia y voltaje observados en la Tabla 2 y fueron visualizadas en el ploteo de Arduino SAMD y en el osciloscopio. 

Primero, se realizó una prueba para determinar el efecto del ruido generado en la señal a partir de su visualización en el ploteo en Arduino. El primer resultado se evidencia en la Figura 4a, la cual muestra lo que se capturó cuando se apagó el generador de señales, en la que el Arduino solo pudo detectar el ruido ambiental presente. Posteriormente, al encender el generador de señales y utilizar un circuito que incluye un filtro RC, se logró modificar la señal de manera significativa, como se ilustra en la Figura 4b. Al remover el capacitor del circuito, como se muestra en la Figura 5, la señal adquirió una forma más cercana a una onda sinusoidal. Sin embargo, se observa una cantidad considerable de ruido en los bordes de la señal.
</div>

<div align="center">

| (a) | (b) | 
| ------------ | ------------ | 
| <image width="500" height="200" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/45044a5e-2595-4701-a666-084410e6ff43"> | <image width="500" height="200" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/df220ad8-b001-4888-82f2-220e2a1aebe3"> | 

</div>
<p align="center"><i>Figura 4. Señal obtenida para la prueba preliminar</i></p>


<p align="center">   
<image width="500" height="350" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/ca1d045e-d375-419a-8072-37d10e8784fc">
<p align="center"><i>Figura 5. Señal obtenida de onda recortada (sin capacitor)</i></p>

<div align="justify">
Luego de dichas pruebas iniciales, se realizó la comparación de las señales graficadas del Arduino IDE con las gráficas obtenidas del osciloscopio para los cuatro tipos de señales: sinusoidales, cuadradas, rampas y pulsos. Asimismo, evaluó el comportamiento del filtro RC junto a la señal obtenida, por lo que se ploteo en el Arduino IDE las 4 señales provenientes del generador.
</div>
<a name="sinusoidal"></a>

### Señal sinusoidal
<div align="center">

| Arduino IDE | Osciloscopio | 
| ------------ | ------------ | 
|  <image width="500" height="200" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/13020895-14d3-438b-a9d5-94a796b466c7"> | <image width="500" height="200" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/c881f0b5-907b-4ece-8c13-ca5993d1807e"> | 
</div>
<p align="center"><i>Figura 6. Señal sinusoidal - Voltaje: 1.5V , Frecuencia: 3Hz</i></p>
<a name="cuadrada"></a>

### Señal cuadrada
<div align="center">

| Arduino IDE | Osciloscopio | 
| ------------ | ------------ | 
| <image width="500" height="200" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/18fc6a55-4988-4a21-9f29-ad54eb8a82bf"> | <image width="500" height="200" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/1e6bf875-2d0d-4e15-9270-9b9c87d6fe26"> | 

</div>
<p align="center"><i>Figura 7. Señal cuadrada - Voltaje: 1.5V , Frecuencia: 3Hz</i></p>
<a name="rampa"></a>

### Señal rampa
<div align="center">

| Arduino IDE | Osciloscopio | 
| ------------ | ------------ | 
| <image width="500" height="200" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/81ff90d0-ef88-4ce6-b85e-22c0f99607a2"> | <image width="500" height="200" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/8195df3e-7476-44f4-8a10-da68e06fb99c"> | 
</div>
<p align="center"><i>Figura 8. Señal rampa - Voltaje: 1.5V , Frecuencia: 3Hz</i></p>
<a name="pulso"></a>

### Señal pulso
<div align="center">

| Arduino IDE | Osciloscopio | 
| ------------ | ------------ | 
| <image width="500" height="200" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/e4cbc5ad-4696-47dc-96df-0a29642682a3"> | <image width="500" height="200" src ="https://github.com/sofiacespedes22/ISB_2024_G8/assets/164541825/a9269650-c215-438b-8878-47f41806ce39"> | 
</div>
<p align="center"><i>Figura 9. Señal pulso - Voltaje: 1.5V , Frecuencia: 3Hz</i></p>

<div align="justify">
Podemos observar, a partir de la comparación, que existen diferencias significativas entre las señales graficadas pues si bien las graficadas en el Arduino IDE presenta las formas deseadas, no llegan a ser las requeridas. A continuación, hemos considerado las siguientes fuentes de error como motivos de las diferencias evidenciadas: 
</div>

<a name="error"></a>
### Fuentes de error
- **Ruido**:
  - Interferencia eléctrica: Los componentes cercanos pueden generar interferencia eléctrica en los microcontroladores, especialmente en entornos con muchos componentes. Esto puede introducir ruido en las mediciones <sup>[1](https://www.watlow.com/es-es/blog/posts/guide-to-electrical-noise)</sup> <sup>[2](https://www.cablesrct.com/blog-cables-rct-es/2681-las-interferencias-electromagneticas#:~:text=Una%20interferencia%20electromagnética%20)</sup>.
  - Condiciones ambientales: Factores ambientales como la temperatura, la humedad y la interferencia electromagnética pueden afectar la calidad de las mediciones <sup>[3](https://www.digikey.com/es/articles/combating-environmental-impact-in-the-electronics-components-industry)</sup>.
  - Ruido generado por la medición por contacto entre el cable y el punto del osciloscopio: Durante la medición, el contacto entre el cable y el punto del osciloscopio pudo haber introducido ruido en la señal, especialmente debido a movimientos o interferencias físicas en este punto de contacto. Esto puede causar fluctuaciones en la señal medida y afectar la precisión de las mediciones <sup>[4](http://dx.doi.org/10.13140/2.1.1678.3688)</sup> .
- **Valor del condensador**: El valor del condensador, al ser un valor grande de 470 uF, actúa como un filtro pasa altas junto con la resistencia de pull-up del Arduino, formando así un filtro RC <sup>[5](http://132.248.52.100:8080/xmlui/handle/132.248.52.100/14284)</sup>. Sin embargo, debido a su gran tamaño, este filtro tiende a atenuar las frecuencias bajas que estamos evaluando, dejando únicamente la señal de ruido como resultado observable.
- **Frecuencias de muestreo**: La frecuencia de muestro es un parámetro esencial al momento de generar una señal por el generador de señales ya que una inadecuada podría generar ruido en la evaluación de la señal. Si la frecuencia de muestreo es demasiado baja en comparación con la frecuencia de la señal original, puede producirse aliasing, lo que distorsiona la representación de la señal <sup>[6](https://doi.org/10.1016/B978-0-12-385920-4.00005-9)</sup>. Además, una frecuencia de muestreo insuficiente puede provocar la pérdida de información de la señal, lo que afecta la precisión de las mediciones. Por ello es importante elegir una frecuencia de muestreo apropiada pues brinda estabilidad y precisión de las mediciones, permitiendo una reconstrucción de la onda original.

<a name="referencias"></a>

## Referencias bibliográficas
[1]“Una guía para el ruido eléctrico | Watlow”. Global Supplier of Industrial Electric Thermal Solutions | Watlow. https://www.watlow.com/es-es/blog/posts/guide-to-electrical-noise

[2]“Las interferencias electromagnéticas - Cables RCT”. Cables RCT - Fabricante de cables eléctricos de baja tensión - Cables RCT. Disponible: https://www.cablesrct.com/blog-cables-rct-es/2681-las-interferencias-electromagneticas#:~:text=Una%20interferencia%20electromagnética%20

[3] S. Raeker. “Lucha contra el impacto ambiental en la industria de los componentes electrónicos”. DigiKey. Disponible: https://www.digikey.com/es/articles/combating-environmental-impact-in-the-electronics-components-industry

[4] CALIDAD DEL SERVICIO DE ENERGÍA ELÉCTRICA. MANIZALES: Cent. Publicaciones Univ. Nac. Colomb. Sede Manizales, 2006.

[5] G. Ellis, "Chapter 5 - The z-Domain," in Control System Design Guide (Fourth Edition), G. Ellis, Ed. Butterworth-Heinemann, 2012, pp. 73-96. [Online]. Available: https://doi.org/10.1016/B978-0-12-385920-4.00005-9

[6] G. Ellis, "Chapter 5 - The z-Domain," in Control System Design Guide (Fourth Edition), G. Ellis, Ed. Butterworth-Heinemann, 2012, pp. 73-96. [Online]. Available: https://doi.org/10.1016/B978-0-12-385920-4.00005-9
