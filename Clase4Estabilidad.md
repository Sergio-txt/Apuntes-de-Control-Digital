# Estabilidad en Sistemas Discretos
En sistemas discretos, donde las señales y las operaciones se realizan en intervalos de tiempo discretos, la estabilidad se refiere a la capacidad del sistema para mantener su comportamiento deseado y no diverger hacia valores incontrolables o inestables con el tiempo. A diferencia de los sistemas continuos, donde se emplean métodos de análisis basados en la transformada de Laplace, los sistemas discretos utilizan herramientas como la transformada Z y el análisis de los polos y ceros en el dominio Z para evaluar su estabilidad

## Índice
1. Estabilidad Absoluta
2. Espacios de LaPlace y Z
3. Métodos de Evaluación de Estabilidad
4. Estabilidad Asintótica
5. Estabilidad BIBO
6. Ejercicios
7. Conclusiones


## 1. Estabilidad Absoluta
La estabilidad absoluta en sistemas discretos se refiere a la capacidad del sistema para mantenerse estable frente a perturbaciones o condiciones iniciales, es decir, un sistema discreto es estable si, tras una perturbación, su salida no crece sin límite y se mantiene acotada.

| Aspecto 	| Sistemas Continuos 	| Sistemas Discretos 	|
|:---:	|:---:	|:---:	|
|      Espacio de Análisis 	| Plano s (Transformada de LaPlace) 	| Plano Z (Transformada Z) 	|
| Criterio de Estabilidad 	| Polos en el semiplano izquierdo (Re(s) < 0) 	| Polos dentro del círculo unitario 	|
| Comportamiento de los Polos 	| Polos con partes reales negativas aseguran que la respuesta se amortigua con el tiempo 	| Polos dentro del círculo unitario aseguran que la respuesta se atenúa con el tiempo 	|

## 2. Espacios de LaPlace y Z
La Transformada de LaPlace es una técnica matemática comúnmente empleada para examinar sistemas lineales invariantes en el tiempo, tales como mecanismos, circuitos eléctricos y sistemas de control.

## 3. Métodos de Evaluación de Estabilidad


## 4. Estabilidad Asintótica


💡**Ejemplo 1:** si se va a representar la ecuación de la ley de Ohm se puede mostrar así $R=\frac{V}{I}$ o también,

$$R=\frac{V}{I}$$

## 6. Figuras
Todas las figuras que incluya deben ser generadas por ustedes, **no utilizar las figuras de las presentaciones**. Para incluir figuras puede seguir los siguientes pasos:
* Primero escribimos ![]().
* Después escribimos, dentro de los corchetes, el texto alternativo. Este es opcional y solo entra en acción cuando no se puede cargar la imagen correctamente.
* Después escribimos, dentro de los paréntesis, la ubicación del archivo (ya sea una url o una ubicación dentro de algun folder local). Se recomienda poner las imágenes en una carpeta que se llame imágenes dentro del repositorio github para que no tengan problemas al cargar las imágenes.

💡**Ejemplo 2:**

![Figura de prueba](images/plantilla/Captura2.PNG)

Figura 1. Figura de prueba

Incluya la respectiva etiqueta a modo de descripción de la figura y mantenga numeración consecutiva para todas las figuras de la clase.

## 5. Estabilidad BIBO
En caso de necesitar la inclusión de tablas para organizar información se recomienda el uso de la herramienta del siguiente enlace https://www.tablesgenerator.com/markdown_tables , la cual permite organizar la información dentro de la tabla y genera el código markdown automáticamente:

💡**Ejemplo 3:** 

| **Resultado** | **x = número de intentos hasta primer éxito** |
|---------------|-----------------------------------------------|
|       S       |                       1                       |
|       FS      |                       2                       |
|      FFS      |                       3                       |
|      ...      |                      ...                      |
|    FFFFFFS    |                       7                       |
|      ...      |                      ...                      |

Tabla 1. Tabla de ejemplo

Cada tabla debe llevar la etiqueta que describa su contenido y numeración consecutiva para todas las tablas

## 6. Ejercicios
Teniendo en cuenta que el curso requiere del desarrollo de código matlab, c, c++ u otro. Si requiere incluir pequeños segmentos de código en los apuntes hágalos de la siguiente manera:

💡**Ejemplo 4:**
```
var sumar2 = function(numero) {
  return numero + 2;
}
```

## 7. Conclusiones
Deben agregar 2 ejercicios con su respectiva solución, referentes a los temas tratados en cada una de las clases. Para agregar estos, utilice la etiqueta #, es decir como un nuevo título dentro de la clase con la palabra 'Ejercicios'. Cada uno de los ejercicios debe estar numerado y con su respectiva solución inmediatamente despues del enunciado. Antes del subtitulo de cada ejercicio incluya el emoji 📚


## Referencias
Agregue un subtítulo al final donde pueda poner todas las referencias consultadas incluyendo el origen o fuente de los ejercicios planteados. Tambien dentro del texto referencie los textos o artículos consultados y las figuras y tablas dentro de la explicación de las mismas.
