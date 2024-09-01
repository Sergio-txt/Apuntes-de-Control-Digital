# Transformada Z de adelantos y atrasos
Una herramienta matemática fundamental para el análisis y diseño de sistemas de control digital es la Transformada Z. La Transformada Z permite convertir ecuaciones en diferencias, que describen la dinámica de sistemas discretos, en expresiones algebraicas más sencillas, de manera similar a la aplicación de la Transformada de Laplace en sistemas continuos. Esto facilita el diseño de controladores digitales que operan en tiempo discreto y el análisis de características del sistema como la estabilidad y el comportamiento transitorio. En el campo de la ingeniería, la Transformada Z es esencial para comprender cómo reaccionan los sistemas a diversas entradas y maximizar su rendimiento en aplicaciones donde las señales se muestran y procesan digitalmente, como en microcontroladores y sistemas de control automatizados.

## Indice
1. Representación matemática de los sistemas discretos
2. Solucion de Ecuaciones en Diferencias
3. Transformada Z
4. Función de transferencia discreta
5. Aplicaciones Prácticas y Ejercicios
6. Conclusiones

## 1. Representación matemática de los sistemas discretos
### 1.1. *Ecuación en Diferencias:* Una ecuación que muestra la relación entre los valores consecutivos de una secuencia y las diferencias entre ellos. A menudo se reorganizan como una fórmula recursiva para que la salida de un sistema pueda calcularse a partir de la señal de entrada y salidas pasadas.


### 1.2. *Ecuaciones en Diferencias No Lineales:* Las ecuaciones en diferencias lineales son aquellas en las que la relación entre las variables es lineal. Esto significa que cada término de la ecuación es una función lineal de la variable de estado o de entrada.Estas ecuaciones se pueden expresar en una forma general como:
$$\[y(k) + a_1 y(k-1) + a_2 y(k-2) + \dots + a_n y(k-n) = b_0 u(k) + b_1 u(k-1) + \dots + b_m u(k-m)\]$$
>Donde:
* y(k) es la salida en el instante k.
* u(k) es la entrada en el instante k.
* $$\[ y(k) + a_1 y(k-1) + a_2 y(k-2) + \dots + a_n y(k-n) = b_0 u(k) + b_1 u(k-1) + \dots + b_m u(k-m) \]$$

### 1.3. *Ecuaciones en Diferencias Lineales:*
Las ecuaciones en diferencias no homogéneas incluyen un término que no depende de la variable de estado, como una entrada o una fuerza externa. Su forma general es:
$$y(k) + a_1 y(k-1) + a_2 y(k-2) + \dots + a_n y(k-n) = b_0 u(k) + b_1 u(k-1) + \dots + b_m u(k-m)$$
Las ecuaciones homogéneas describen sistemas que no tienen una entrada externa y son útiles para estudiar la respuesta natural del sistema.

### 1.4. *Ecuaciones en Diferencias No Homogéneas:*
Las ecuaciones en diferencias no homogéneas incluyen un término que no depende de la variable de estado, como una entrada o una fuerza externa. Su forma general es:
$$y(k) + a1 * y(k-1) + a2 * y(k-2) + ... + an * y(k-n) = b0 * u(k) + b1 * u(k-1) + ... + bm * u(k-m)$$
Donde f(k) es una función que representa la entrada o una perturbación externa. Estas ecuaciones describen sistemas que responden a un estímulo exter

## 2. Solucion de Ecuaciones en Diferencias
### 2.1. *Métodos Iterativos:*
Este método consiste en calcular los valores sucesivos de la variable de estado de manera recursiva, utilizando los valores iniciales conocidos y aplicando la ecuación en diferencias repetidamente. Es especialmente útil para ecuaciones en diferencias lineales de primer orden o de bajo orden.
Ejemplo: Si tienes una ecuación en diferencias de primer orden:
$$y(k) = 0.5 \cdot y(k-1) + u(k)$$
Puedes calcular $y(k)$ para $k = 1, 2, 3 ...$ usando un valor inicial $y(0)$ y la secuencia de valores de $u(k)$

### 2.2. *Transformada Z de ecuacioens en diferencias*
La Transformada Z es una herramienta poderosa para resolver ecuaciones en diferencias, especialmente en el análisis de sistemas de control digital. Este método convierte la ecuación en diferencias en una ecuación algebraica en el dominio Z, que es más fácil de manipular.

>Pasos básicos:
* Aplicar la Transformada Z: Conviertes la ecuación en diferencias en una ecuación en términos de la variable Z.
* Resolver la ecuación algebraica: Despejas la variable de interés en el dominio Z.
* Aplicar la Transformada Z inversa: Conviertes la solución obtenida en el dominio Z de vuelta al dominio del tiempo discreto, obteniendo la secuencia de valores de la variable de estado.

Ejemplo: Para la ecuación en diferencias:
$$yh(k) - 0.5 \cdot y(k-1) = u(k)$$
La solución general de la ecuación homogénea asociada es:
$$Y(z) - 0.5z^{-1} Y(z) = U(z)$$
Despejando $Y(z)$:
$$Y(z) = \frac{U(z)}{1 - 0.5z^{-1}}$$
Luego, aplicamos la Transformada Z inversa para encontrar $y(k)$

## 2. Transformada Z
### 2.1. *Transformada Z de un Atraso*
La Transformada Z es una herramienta matemática utilizada en el análisis y diseño de sistemas discretos. Es particularmente útil en el procesamiento digital de señales y en el control de sistemas discretos.
Dada una secuencia de tiempo discreto $x[n]$, la Transformada Z de $x[n]$ se define como:
$$X(z) = \sum_{n=-\infty}^{\infty} x[n] z^{-n}$$
donde $Z$ es una variable compleja.
### 2.2. *Atraso de una Secuencia*
Un atraso de $k$ unidades en una secuencia discreta $x[n]$ se representa como $x[n−k]$. Esto significa que cada valor de la secuencia se retrasa $k$ pasos en el tiempo.

Para encontrar la Transformada Z de la secuencia retrasada $x[n−k]$, utilizamos la propiedad del atraso de la Transformada Z:
$$\mathcal{Z}\{x[n - k]\} = z^{-k} X(z)$$
>Donde
* $Z{⋅}$ denota la Transformada Z
* $x[n−k]$ es la secuencia original retrasada por $k$ unidades
* $X(z)$ es la Transformada Z de la secuencia original $x[n]%
* $z^{-k}$ es un factor de escala que representa el atraso.

### 2.2. Transformada Z de un Adelanto
En el contexto de señales y sistemas discretos, un adelanto en una secuencia se refiere a la operación en la que cada valor de la secuencia se avanza o se adelanta en el tiempo.
Dada una secuencia discreta $x[n]$, un adelanto de $k$ unidades en la secuencia se representa como $x[n+k]$. Esto significa que cada valor de la secuencia se adelanta 
$k$ pasos en el tiempo.
Para encontrar la Transformada Z de la secuencia adelantada  $x[n+k]$, utilizamos la propiedad del adelanto de la Transformada Z:
$$\mathcal{Z}\{x[n + k]\} = z^k X(z)$$

>Donde
* $Z{⋅}$ denota la Transformada Z
* $x[n+k]$ es la secuencia original adelantada por $k$ unidades
* $X(z)$ es la Transformada Z de la secuencia original $x[n]%
* $z^{k}$ es un factor de escala que representa el adelanto.


### 2.3 Funcion de tranferencia discreta
La función de transferencia de un sistema discreto es una representación matemática que relaciona la entrada y la salida del sistema en el dominio Z. Se define como el cociente entre la Transformada Z de la salida y la Transformada Z de la entrada, bajo condiciones iniciales nulas.
Si $X(z)$ es la Transformada Z de la entrada $x[n]$ y $Y(z)$ es la Transformada Z de la salida $y[n]$, la función de transferencia $H(z)$ se define como:
$$H(z) = \frac{Y(z)}{X(z)}$$

>Donde
* $Y(z)$ es la Transformada Z de la salida del sistema.
* $X(z)$ es la Transformada Z de la entrada del sistema.

### 2.4 Pasar de una función de transferencia en atraso a adelanto
Supongamos que tienes una función de transferencia en el dominio Z que involucra un atraso. La función de transferencia en atraso es:
$$H(z) = \frac{Y(z)}{X(z)}$$
donde $Y(z)$ y $X(z)$ están relacionadas a través del atraso en el tiempo.
$z^{-k} \text{ a } \frac{a}{z^k}$ donde $k$ es el número de unidades de tiempo en el que se adelanta la secuencia.

#### 2.4.1 Proceso 
>Escribe la Función de Transferencia Original:
Supongamos que tienes una función de transferencia en atraso que tiene el siguiente formato:





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
1.CHAPRA, S.C. y CANALE, R.P M´etodos Numéricos para Ingenieros. McGraw-Hill, 1987.
2.

