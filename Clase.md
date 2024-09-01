# Transformada Z de adelantos y atrasos
La Transformada Z es una herramienta matemática fundamental en el análisis y diseño de sistemas de control digital. Al igual que la Transformada de Laplace se utiliza para sistemas continuos, la Transformada Z permite convertir ecuaciones en diferencias, que describen la dinámica de sistemas discretos, en expresiones algebraicas más manejables. Esto facilita el estudio de las propiedades del sistema, como la estabilidad y el comportamiento transitorio, así como el diseño de controladores digitales que operan en tiempo discreto. En el contexto de la ingeniería, la Transformada Z es crucial para comprender cómo los sistemas responden a diferentes entradas y cómo optimizar su rendimiento en aplicaciones donde la señal es muestreada y procesada digitalmente, como en los microcontroladores y sistemas de control automatizado.

## Indice
1. Señales Analógicas y Digitales
2. Procedimiento de Conversión A/D
3. Procedimiento de Conversión D/A
4. Implementación Física y Modelos Matemáticos
5. Aplicaciones Prácticas y Ejercicios
6. Conclusiones

## 1. Señales Analógicas y Digitales

>🔑 *Señal Analóga:* Las señales analógicas son continuas tanto en el tiempo como en la amplitud, lo que significa que pueden llegar a tomar cualquier valor dentro de un rango continuo, representando información de manera fluida e ininterrumpida. 

![Señal Analóga](http://xkiller-damndx.mex.tl/imagesnew2/0/0/0/2/1/3/9/8/2/5/Standing_wave_2.gif)

Figura 1. Señal Analóga

>🔑 *Señal Digital:* Son discretas tanto en tiempo como en amplitud, puesto que representan información en forma de secuencias de valores binarios (0 y 1), obtenidas mediante la conversión de señales analógicas.


Las subsecciones pueden utilizarse para sub dividir ciertos temas que se tienen en clases, por ejemplo si se está trabajandolos conversores D/A, puede ser necesario subdividir este en circuito de resistencias ponderadas y circuito de escalera R2R. 
### 3.1. Título de subsecciones
Para la creación de estas subsecciones debe utilizar un tamaño de letra más pequeño, por lo tanto utilice la etiqueta '###' 
### 3.2. Numeración de subsecciones
Siga la numeración de la sección seguida de un punto y luego el número de la subsección.

## 4. Ejemplos
Si en algún caso pretende dar un ejemplo explicativo ya sea a través de texto o através de ecuaciones matemáticos, utilizar la palabra 'Ejemplo' seguido de una numeración consecutiva dentro de la clase. Utilice el emoji 💡 antecediendo la palabra.

## 5. Ecuaciones
Para la edición de ecuaciones debe utilizar la etiqueta '$$' al comienzo y final de la ecuación para que la ecuación quede centrada ocupando una línea. Si se quiere que la ecuación quede integrada en el texto debe utilizar la etiqueta '$' al comienzo y final de la ecuación. Las ecuaciones pueden ser editadas utilizando el código LATEX, en el siguiente enlace encuentran un editor de ecuaciones que les genera el código. http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp . Sin embargo hay muchas otras herramientas que pueden utilizar para esto.

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

## 7. Tablas
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

## 8. Código
Teniendo en cuenta que el curso requiere del desarrollo de código matlab, c, c++ u otro. Si requiere incluir pequeños segmentos de código en los apuntes hágalos de la siguiente manera:

💡**Ejemplo 4:**
```
var sumar2 = function(numero) {
  return numero + 2;
}
```

## 9. Ejercicios
Deben agregar 2 ejercicios con su respectiva solución, referentes a los temas tratados en cada una de las clases. Para agregar estos, utilice la etiqueta #, es decir como un nuevo título dentro de la clase con la palabra 'Ejercicios'. Cada uno de los ejercicios debe estar numerado y con su respectiva solución inmediatamente despues del enunciado. Antes del subtitulo de cada ejercicio incluya el emoji 📚

## 10. Conclusiones
Agregue unas breves conclusiones sobre los temas trabajados en cada clase, puede ser a modo de resumen de lo trabajado o a indicando lo aprendido en cada clase

## 11. Referencias
1.Barrero Mendoza, Oscar. Sistemas de control digital. Universidad de Ibagué, 2021. Digitalia.
2.Chen, C. T. Analog and Digital control design. Saunders College Publishing.

