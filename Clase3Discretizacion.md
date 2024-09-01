# Discretización de controladores Analógicos

## Indice
1. Discretización de señales Analógicas
2. Método de Invarianza al impulso
3. Transformada Z
4. Sistemas Causales y no causales
5. Tiempo muerto en sistemas discretos
6. Conclusiones
7. Referencias



## 1. Discretización de señales Analógicas
La discretización de señales analógicas es el proceso mediante el cual una señal continua en el tiempo y en amplitud se convierte en una señal discreta, que es una secuencia de valores en instantes específicos. Este proceso es esencial para el procesamiento digital de señales, ya que permite que las señales analógicas sean manipuladas y analizadas utilizando sistemas digitales como computadoras y microcontroladores.

## 2. Método de Invarianza al impulso
Es una técnica para obtener una función de transferencia digital a partir de una función de transferencia analógica. La idea central es que la respuesta al impulso de un filtro analógico se puede mapear directamente a la respuesta al impulso de un filtro digital mediante una transformación.
>🔑*Proceso de Transformación:*
* Obtención de la Respuesta al Impulso Analógica:
Primero, se determina la respuesta al impulso del filtro analógico. La respuesta al impulso 
 $h_a(t)$ es la salida del filtro cuando se aplica un impulso unitario $δ(t)$ como entrada.

>🔑*Transformación a la Respuesta al Impulso Digital:*
*La respuesta al impulso analógica  $h_a(t)$ se convierte en una secuencia discreta aplicando un muestreo en el tiempo. Esto se hace evaluando 
 $h_a(t)$  en intervalos de tiempo $T$, donde $T$ es el período de muestreo del sistema digital.

>🔑*Transformación de la Función de Transferencia:*
* La función de transferencia del filtro digital $H(z)$  se obtiene a partir de la transformada Z de la respuesta al impulso digital. Esto se puede hacer utilizando la transformada Z de la secuencia discreta obtenida en el paso anterior.




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
Agregue un subtítulo al final donde pueda poner todas las referencias consultadas incluyendo el origen o fuente de los ejercicios planteados. Tambien dentro del texto referencie los textos o artículos consultados y las figuras y tablas dentro de la explicación de las mismas.
