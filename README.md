# Fundamentos y Procedimientos de la Conversión A/D y D/A en Control Digital
La conversión entre señales analógicas y digitales es un proceso fundamental en los sistemas de control digital, en donde se requiere adaptar señales continuas provenientes del mundo físico a un formato que pueda ser procesado por sistemas digitales, y viceversa, por esta razón, dentro del ámbito de la ingeniería, este proceso reúne la recolección de datos a través de sensores que interactúan con señales, las cuales deben ser transformadas adecuadamente para que los controladores digitales puedan manejarlas de manera eficiente. En este sentido, la conversión A/D permite convertir una señal analógica, como temperatura, velocidad o humedad, en una señal digital para su procesamiento, mientras que la conversión D/A hace posible que las señales digitales se conviertan nuevamente a analógicas para controlar dispositivos en el mundo real.

## Indice
1. Señales Analógicas y Digitales
2. Procedimiento de Conversión A/D
3. Procedimiento de Conversión D/A
4. Modelos Matemático
5. Aplicaciones Prácticas y Ejercicios
6. Conclusiones
## 1. Señales Analógicas y Digitales
Las señales pueden clasificarse en dos tipos fundamentales: analógicas y digitales, cada tipo tiene características distintivas que afectan su uso en diversos sistemas de comunicación y procesamiento.

A continuación se detallan las diferencias y características fundamentales de ambos tipos de señales:

>🔑 *Señal Analóga:* Las señales analógicas son continuas tanto en el tiempo como en la amplitud, lo que significa que pueden llegar a tomar cualquier valor dentro de un rango continuo, representando información de manera fluida e ininterrumpida. [1] 

![Señal Analóga](http://xkiller-damndx.mex.tl/imagesnew2/0/0/0/2/1/3/9/8/2/5/Standing_wave_2.gif)

Figura 1. Señal Analóga

>🔑 *Señal Digital:* Son discretas tanto en tiempo como en amplitud, puesto que representan información en forma de secuencias de valores binarios (0 y 1), obtenidas mediante la conversión de señales analógicas. [2]

![Señal Analóga](https://miro.medium.com/v2/resize:fit:1000/1*T05QpHC6DaUl7-9Xrqo5IA.gif)

Figura 2. Digital

#### Comparativa entre señales
| Características 	| Señal Analogica 	| Señal Digital 	|
|:---:	|:---:	|:---:	|
| Continuidad 	| Fluida y continua, sin saltos. 	| Discreta, con intervalos definidos. 	|
| Susceptibilidad al Ruido 	| Alta, susceptible a interferencias y distorsiones. 	| Baja, más robusta frente a perturbaciones. 	|
| Procesamiento y Almacenamiento 	| Más difícil de procesar y almacenar debido a la continuidad. 	| Fácil de procesar y almacenar utilizando sistemas digitales. 	|
| Calidad de Información 	| Puede perderse debido a ruido y distorsión. 	| Mantiene la integridad con menos pérdida. 	|

## 2. Procedimiento de Conversión A/D
El proceso de conversión A/D se realiza en tres etapas: muestreo, cuantización y codificación.
### Muestreo
El muestreo es el proceso mediante el cual una señal analógica continua en el tiempo es capturada en intervalos de tiempo discretos, es decir que implica tomar "instantáneas" de la señal en momentos específicos, con el objetivo de obtener una secuencia de valores que puedan ser utilizados en sistemas digitales, por tanto hay dos aspectos que son esenciales en este proceso ya que incluye la frecuencia de muestreo, que es la tasa a la que se capturan los valores de la señal analógica, y el período de muestreo, que es el intervalo de tiempo entre cada muestra. 

#### Teorema del muestreo
En el teorema del muestreo establece que para representar correctamente una señal analógica en forma digital, la frecuencia de muestreo debe ser al menos el doble de la frecuencia máxima de la señal continua. Este principio, tambien conocido como el teorema de Nyquist-Shannon, asegura que la señal digital resultante conserve toda la información de la señal original, por tanto, si la frecuencia de muestreo es insuficiente, pueden surgir problemas como el aliasing, donde las frecuencias altas se confunden con frecuencias bajas, distorsionando la señal y comprometiendo la calidad de la representación digital.

![Señal Analóga](https://miro.medium.com/v2/resize:fit:1000/1*T05QpHC6DaUl7-9Xrqo5IA.gif)
![Señal Analóga](https://github.com/Evellyn27/Apuntes-de-Control-Digital/blob/3c0e776d83616f144ae21ed4f9f465e3fe096eea/Screenshot%202024-08-31%20201541.png)


### Cuantización
### Codificación
## 3. Procedimiento de Conversión D/A

## 4. Modelo Matemático

## 5. Aplicaciones Prácticas y Ejercicios

## 6. Conclusiones

## Referencias
[1] “Comunicaciones”. Tipos y Modos de Comunicaciones. Accedido el 28 de agosto de 2024. [En línea]. Disponible: http://xkiller-damndx.mex.tl/frameset.php?url=/1488142_Caracteristicas-de-las-senales-y-Conceptos-de-Ondas.html

[2] F. Miyara, CONVERSORES D/A Y A/D, 2a ed. 2004.
