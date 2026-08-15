# Clase 28 de Julio / 2026

Decimal:  13
Binario:  1101

13 ÷ 2 = 6, residuo 1
6  ÷ 2 = 3, residuo 0
3  ÷ 2 = 1, residuo 1
1  ÷ 2 = 0, residuo 1
(Residuos de abajo hacia arriba)

## Ejemplo:

- 87 ÷ 2 = 43, residuo 1
- 43 ÷ 2 = 21 , residuo 1
- 21 ÷ 2 = 10 , residuo 1
- 10 ÷ 2 = 5 , residuo 0
- 5 ÷ 2 = 2 , residuo 1
- 2 ÷ 2 = 1 , residuo 0
- 1 ÷ 2 = 0 , residuo 1
- 0

## Nota:

- 87 en base 10 = 01010111 en base 2

## Ejemplo 2:

- | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
- |  0  |  1 |  1 |  0 | 0 | 1 | 0 | 0 |

- 'A' = 65 = 01000001 (en binario) → almacenado en 1 byte.

- |  0  |  1 |  1 |  1 | 1 | 1 | 1 | 1 |base 2 = 127
- |  1  |  0 |  0 |  0 | 0 | 0 | 0 | 1 | = -127

## Complementos:

- 000 = 111
- 001 = 110
- 010 = 101
- 011 = 100
- 100 = 011
- 101 = 010
- 110 = 001
- 111 = 000

**De binario a decimal:**

Para convertir 1011 a decimal:

$1*(2^3) + 0*(2^2) + 1*(2^1) + 1*(2^0) = 8 + 0 + 2 + 1 = 11$

### Ejercicios

1. Convierte el número decimal 22 a binario.
2. ¿Cuál es el resultado en decimal del número binario 10110?

### Solución:

1)
- 22 ÷ 2 = 11, residuo 0
- 11 ÷ 2 = 5 , residuo 1
- 5 ÷ 2 = 2 , residuo 1
- 2 ÷ 2 = 1 , residuo 0
- 1 ÷ 2 = 2 , residuo 1
- 0

= 10110

2)

$1*(2^4) + 0*(2^3) + 1*(2^2) + 1*(2^1)+ 0*(2^0) = 16 + 0 + 4 + 2 + 0 = 22$

## Ejercicio 1

En la Figura 2 se muestran los diferentes estados que se pueden representar usando una palabra binaria de 3 bits. Responde la pregunta de la imagen: ¿Cuántos estados diferentes se pueden representar usando N bits?

<img width="474" height="304" alt="Untitled" src="https://github.com/user-attachments/assets/50a59559-4e6a-45e9-9110-abc32e98455c" />

Para resolver el ejercicio anterior, intenta con 2 bits, luego con 3 y así sucesivamente. Intenta encontrar una representación matemática para dicha secuencia. 

### Ejercicios

1. ¿Qué número binario representa el carácter 'C' en ASCII?
2. Convierte el número flotante 5.75 a binario (explica los pasos).

### Solución:

1. El carácter 'C' en ASCII corresponde al número decimal 67.

Convertimos 67 a binario:

\[
67 = 64 + 2 + 1
\]

Por lo tanto:

C = $01000011_{2}$

2. Para convertir 5.75 a binario, separamos la parte entera y la decimal.

### 1. Parte entera: 5
- Dividimos entre 2:

5 ÷ 2 = 2, residuo 1
2 ÷ 2 = 1, residuo 0
1 ÷ 2 = 0, residuo 1

Leyendo los residuos de abajo hacia arriba:

$5_{10} = 101_{2}$

### 2. Parte decimal: 0.75
- Multiplicamos por 2 y tomamos la parte entera:

0.75 × 2 = 1.5 → parte entera 1
0.5 × 2 = 1.0 → parte entera 1

Entonces:

$0.75_{10} = 0.11_{2}$

### 3. Unimos ambas partes

$5.75_{10} = 101.11_{2}$

### Resultado final:

$5.75_{10} = 101.11_{2}$

### Ejercicios

1. ¿Cuántos bytes se necesitan para almacenar la palabra “Hola” en ASCII?
2. ¿Cuántos bits hay en 5 KB?

### Solución:

1. En ASCII, C = 67 en decimal.
Convertimos 67 a binario:

67 = 64 + 2 + 1

67 =   $1*(2^6) + 1*(2^1) + 1*(2^0) = 64 + 2 + 1 = 67_{10} = 01000011_2$


2. Convierte el número flotante 5.75 a binario

- Separamos la parte entera y la parte decimal:
- Parte entera: 5
- Dividimos entre 2:

5 ÷ 2 = 2, residuo 1
2 ÷ 2 = 1, residuo 0
1 ÷ 2 = 0, residuo 1

Leyendo los residuos de abajo hacia arriba:

$5_{10} = 101_{2}$

- Parte decimal: 0.75
- Multiplicamos por 2: 0.75 x 2 = 1.5
- Tomamos el 1 y continuamos con 0.5: 0.5 x 2 = 1.0
- Tomamos el 1 y por lo tanto: $0.75_{10} = 0.11_{2}$
- Unimos ambas partes: $5.75_{10} = 101.11_{2}$
- Respuesta: 101.11

### Almacenamiento Digital de Datos

### ¿Cómo se almacenan los datos?

Los datos se almacenan en la memoria y en dispositivos de almacenamiento como secuencias de bits. La unidad básica es el **bit**, pero normalmente se agrupan en **bytes** (8 bits).

- **Palabra:** Unidad de datos que maneja el procesador (puede ser 16, 32 o 64 bits).
- **Unidades de almacenamiento:** 1 byte = 8 bits, 1 KB = 1024 bytes, 1 MB = 1024 KB, etc.

**Diagrama de almacenamiento:**

|--bit--|--bit--|--bit--|--bit--|--bit--|--bit--|--bit--|--bit--|
|------------------------- 1 byte ------------------------------|

**Ejemplo:**
Guardar la letra 'A' en memoria:

- 'A' = 65 = 01000001 (en binario) → almacenado en 1 byte.

### Ejercicios

1. ¿Cuántos bytes se necesitan para almacenar la palabra “Hola” en ASCII?
2. ¿Cuántos bits hay en 5 KB?

### Solución:

1. La palabra “Hola” tiene 4 caracteres:
H → 1 byte
o → 1 byte
l → 1 byte
a → 1 byte

Entonces:

4 caracteres x 1 byte = 4 bytes

Respuesta: 4 bytes

2. Usando: 1KB = 1024 bytes
- Y como 1 byte = 8 bits
- Tenemos: 5120 x 8 = 40960 bits

Respuesta: 40.960 bits

### tras Temáticas Relevantes

### Sistema hexadecimal

El sistema hexadecimal (base 16) es usado frecuentemente para representar datos binarios de forma más compacta.

**Conversión:**

- 1111 1111 (binario) = FF (hexadecimal)
- 1010 1100 (binario) = AC (hexadecimal)

<img width="779" height="272" alt="capture_temp" src="https://github.com/user-attachments/assets/7754168d-163e-469e-9ccf-e8a7df808fce" />

### Errores de redondeo y precisión

En los números de punto flotante, no todos los números decimales pueden representarse exactamente, lo que provoca errores de redondeo.

### Codificación de colores

Colores en computadoras suelen representarse en formato RGB, usando valores hexadecimales:

- Rojo: #FF0000
- Verde: #00FF00
- Azul: #0000FF

### Ejercicios

1. Convierte el número decimal 255 a hexadecimal.
2. ¿Cuál es el valor hexadecimal de la secuencia binaria 11010110?

### Solución:

1. Dividimos entre 16: 255 ÷ 16 = 155, residuo 15

- En Hexadecimal: 15 = F
- Entonces:
$255_{10}$ = $FF_{16}$
- Respuesta: FF

2. Separamos el número binario en grupos de 4 bits:

- 1101 y 1010

Convertimos cada grupo:

- $1101_{2}$ = $13_{10}$ = $D_{16}$

Por lo tanto:

$11010110_{2}$ = $DA_{16}$

Respuesta: DA

## Ejercicios Finales de Repaso

1. Explica, en tus propias palabras, por qué es necesario que las computadoras representen los datos en binario.
2. Convierte el número binario 10011011 a decimal y a hexadecimal.
3. Investiga y describe cómo se representa una imagen en formato PNG en el disco.
4. Analiza la siguiente situación: ¿Qué sucede si intentas almacenar un número mayor al que puede representar un byte (por ejemplo, 300)? ¿Cómo lo maneinstrucció

### Solución:

1. Las computadoras utilizan binario porque sus componentes electrónicos trabajan principalmente con dos estados, que se pueden representar como 0 y 1. Con estos dos valores pueden representar números, letras, imágenes, sonidos y cualquier otro tipo de información.

2. ### A decimaal:

$10011011_{2}$  =  $1*(2^7) + 0*(2^6) + 0*(2^5) + 1*(2^4) + 1*(2^3) + 0*(2^2) + 1*(2^1)+ 1*(2^0) = 128 + 16 + 8 + 2 + 1 = 155$

Por lo cual:

$10011011_{2}$  =   $155_{10}$

### A Hexadecimal:

Separamos en grupos de 4:

- 1001 y 1011
- 1001 = 9
- 1011 = B

Por lo tanto:

$10011011_{2}$ = $9B_{16}$

Respuesta: 155 en decimal y 9B en hexadecimal

3. Una imagen PNG se almacena en el disco como un archivo formado por datos binarios. En este, el archivo contiene información sobre la imagen como su ancho, alto, colores y otros datos, además de los datos de los píxeles.
- La PNG utiliza compresión sin pérdida, por lo que puede reducir el tamaño del archivo sin perder información de la imagen. Entonces, cuando un programa abre el PNG, interpreta esos datos binarios y reconstruye la imagen para mostrarla en pantalla.
- En resumen, aunque nosotros vemos una imagen, en el disco realmente está almacenada como una secuencia de bytes (0 y 1).

4. Python puede manejar 300 como un entero normal, pero no puede representarlo en un solo byte sin utilizar más espacio, es decir, un byte puede representar valores de 0 a 255 cuando se utiliza sin signo.

Por ejemplo:

$255_{10}$   =   $11111111_{2}$

Pero 300 es mayor que 255, por lo que no cabe en un solo byte.
En Python, un número entero normal (int) no está limitado a un byte. Como resultado se produce un "OverflowError"

# Clase de Algoritmos:

## Símbolos que se utilizan para representar cada operación de un algoritmo con un diagrama de flujo:

## 1. Óvalo 
- Inicio/Fin: Se utiliza para indicar el comienzo y el final de un algoritmo. Todo diagrama de flujo debe iniciar y terminar con este símbolo.

## 2. Rectángulo 
- Proceso: Representa una acción, operación o cálculo que debe realizar el algoritmo, como sumar dos números, asignar un valor o ejecutar una instrucción.

## 3. Paralelogramo 
- Entrada de datos: Se utiliza para representar la entrada o salida de información. Generalmente indica que el usuario ingresa datos o que el sistema muestra un resultado.

## 4. Rombo 
- Condición: Representa una decisión o comparación. Dependiendo de si la condición es verdadera o falsa, el algoritmo sigue un camino diferente.

## 5. Círculo
- Conector: Sirve para unir diferentes partes del diagrama de flujo sin necesidad de trazar líneas muy largas, facilitando su organización y lectura.

## 6. Símbolo de cinta magnética 
- Cinta magnética: Representa el almacenamiento de datos en una cinta magnética. Es un símbolo tradicional que hoy en día se utiliza muy poco.

## 7. Cilindro 
- Disco magnético: Indica que la información se almacena en un disco duro o en una base de datos, es decir, en un medio de almacenamiento permanente.

## 8. Pentágono 
- Conector de página: Se utiliza cuando el diagrama continúa en otra hoja. Permite indicar dónde debe seguir el flujo del algoritmo.

## 9. Flechas 
- Líneas de flujo: Muestran la dirección y el orden en que se ejecutan las instrucciones dentro del diagrama de flujo.

## 10. Símbolo de pantalla o display 
- Mostrar datos: Representa la salida de información en un monitor o pantalla para que el usuario pueda visualizar los resultados.

## 11. Símbolo de documento 
- Enviar datos a impresora: Indica que la información generada por el algoritmo será enviada a una impresora o se obtendrá un documento impreso como salida.

<img width="235" height="425" alt="Captura de pantalla 2026-08-04 101913" src="https://github.com/user-attachments/assets/d9673def-26d9-42e7-b5f4-4bb2f7fcfb93" /> 
<img width="852" height="800" alt="5173492_orig" src="https://github.com/user-attachments/assets/1356c8da-e628-4877-8109-c9b9374dde2f"/>


## Reglas para el uso de diagramas de flujo:

1. Todo diagrama de flujo debe tener un **inicio y** un **fin.** 
2. Las líneas utilizadas para indicar la dirección del flujo del  diagrama deben ser rectas: verticales u horizontales. 
3. Todas las líneas utilizadas para indicar la dirección del flujo  del diagrama deben estar conectadas. La conexión puede  ser a un símbolo que exprese lectura, proceso, decisión,  impresión, conexión o fin del diagrama. 
4. El diagrama de flujo debe construirse de arriba hacia abajo  (*top-down*) y de izquierda a derecha (*left to right* ).
5. La notación utilizada en el diagrama de flujo debe ser  independiente del lenguaje de programación. 
6. Al realizar una tarea compleja, es conveniente poner  comentarios que expresen o ayuden a entender lo que  hayamos hecho. 
7. Si la construcción del diagrama de flujo requiriera más de  una hoja, debemos utilizar los conectores adecuados y  enumerar las páginas correspondientes. 
8. No puede llegar más de una línea a un símbolo  determinado

# Clase 04 de Agosto / 2026


## Ejemplo 1:

<img width="262" height="1092" alt="Ejercicio2" src="https://github.com/user-attachments/assets/f1cd7453-b3fe-4ea0-b623-e5973fea0f51" />


## Ejemplo 2

<img width="712" height="912" alt="Diagrama sin título drawio" src="https://github.com/user-attachments/assets/97d6a1f8-4501-41c6-9dfd-dadf9a8f059b" />


## Operadores Aritméticos:

<img width="170" height="248" alt="Captura de pantalla 2026-08-04 103059" src="https://github.com/user-attachments/assets/ab548734-9bea-4d54-bdb0-4ba3fe49b9e9" />
<img width="235" height="425" alt="Captura de pantalla 2026-08-04 101913" src="https://github.com/user-attachments/assets/b32ef7de-1fa1-42a5-92d4-3b69439bb552" />


# Clase 06 de Agosto / 2026

1. For:
<img width="332" height="235" alt="image" src="https://github.com/user-attachments/assets/5e514b06-fff4-4905-a44b-cde94f16ba0c" />

2. While:
<img width="248" height="253" alt="image (1)" src="https://github.com/user-attachments/assets/01fabc68-f8c8-4b91-b7ff-46619cbafe3c" />

3. Do - While:
<img width="249" height="252" alt="image (2)" src="https://github.com/user-attachments/assets/eef8bd6e-2bf1-4259-b856-dbb5c07cac7f" />

# Ejemplo 1

Contador:
- C = 0
- C = C + 1

Acumulador:
- Ac = 0 <- Suma
- Ac = Ac + N

<img width="527" height="391" alt="image (3)" src="https://github.com/user-attachments/assets/e0a5ebcb-70b2-4a51-8a8f-4538d1fafe58" />

# Ejemplo 2

<img width="638" height="302" alt="image (4)" src="https://github.com/user-attachments/assets/4b3a8ce7-625d-4962-add4-ced77423c41c" />

# Pregunta de Parcial

¿Cual es la diferencia entre un acumulador y el contador?

# Ejemplo 3

<img width="730" height="852" alt="Ese5 drawio" src="https://github.com/user-attachments/assets/db2cba25-3631-4b75-9da2-fa261efd5a5e" />

# Ejercicios de diagramas de flujo

1. Realice un algoritmo para determinar cuánto se debe pagar por equis cantidad de lápices considerando que si son 1000 o más el costo es de $85 cada uno; de lo contrario, el precio es de $90. Represéntelo con el pseudocódigo y el diagrama de flujo.

![Mi Imagen](https://github.com/Sebastian5050942/Toma_notas_Programaci-n/blob/dc005b9b4697ea21751a2f60d8ae1ecf4327b15d/Ese.drawio.png)

2. Un acuario necesita determinar cuántos litros o galones (eso lo decide el usuario) de agua caben en un acuario, pero solo dispone de una cinta métrica (en centímetros). Diseña un algoritmo para solucionar el problema.

![Mi Imagen](https://github.com/Sebastian5050942/Toma_notas_Programaci-n/blob/dc005b9b4697ea21751a2f60d8ae1ecf4327b15d/Ese2.drawio.png)

3. Un almacén de ropa tiene una promoción: por compras superiores a $250 000 se les aplicará un descuento de 15%, de caso contrario, sólo se aplicará un 8% de descuento. Realice un algoritmo para determinar el precio final que debe pagar una persona por comprar en dicho almacén y de cuánto es el descuento que obtendrá. Represéntelo mediante el pseudocódigo y el diagrama de flujo.

![Mi Imagen](https://github.com/Sebastian5050942/Toma_notas_Programaci-n/blob/dc005b9b4697ea21751a2f60d8ae1ecf4327b15d/Ese3.drawio.png)

4. El director de una escuela está organizando un viaje de estudios, y requiere determinar cuánto debe cobrar a cada alumno y cuánto debe pagar a la compañía de viajes por el servicio. La forma de cobrar es la siguiente: si son 100 alumnos o más, el costo por cada alumno es de $65.00; de 50 a 99 alumnos, el costo es de $70.00, de 30 a 49, de $95.00, y si son menos de 30, el costo de la renta del autobús es de $4000.00, sin importar el número de alumnos.

![Mi Imagen](https://github.com/Sebastian5050942/Toma_notas_Programaci-n/blob/dc005b9b4697ea21751a2f60d8ae1ecf4327b15d/Ese4.drawio.png)


# Actividad de Evaluación: Comprensión de Conceptos

## **Consigna tus respuestas en la bitácora**

A continuación, se presentan enunciados relacionados con los temas tratados en el texto. Los estudiantes deben responder si los enunciados corresponden o no con las definiciones o conceptos aprendidos.

### Parte 1: Identificar Algoritmos

Responde si los siguientes enunciados representan un algoritmo. Justifica la respuesta:

1. Una página web.
2. Una receta para hacer un pastel, donde se indican ingredientes y pasos a seguir.
3. "Piensa en un número y multiplícalo por otro".
4. Un manual de instrucciones para armar un mueble, con pasos detallados y un orden claro.
5. Una lista de compras organizada en orden alfabético

### Parte 2: Variables y Constantes

Indica si las siguientes afirmaciones describen una variable o una constante:

1. El valor de la gravedad en la Tierra, 9.8 m/s².
2. La edad de una persona calculada con base en el año actual y su año de nacimiento.
3. La cantidad de dinero en una cuenta bancaria.
4. La velocidad de la luz en el vacío, 299,792,458 m/s.
5. El radio de un círculo.

### Parte 3: Características de los Algoritmos

Responde si los siguientes enunciados cumplen con las características de un algoritmo. Justifica la respuesta:

1. Para elegir la ruta más corta entre varias ciudades, el algoritmo examina rutas candidatas, deteniéndose cuando los cambios en la distancia parecen lo suficientemente pequeños.
2. Suma los números ingresados y muestra el resultado.
3. Un conjunto de pasos para calcular el área de un rectángulo dado su base y altura.
4. El algoritmo cuenta el número de votos obtenidos por cada uno de los candidatos de una elección para presidente. Empieza solicitando el nombre del candidato y finaliza cuando se ingresa el valor -1.

### Parte 4: Comprensión de Herramientas

Indica si las siguientes afirmaciones son ciertas o falsas respecto al pseudocódigo y diagramas de flujo:

1. El pseudocódigo utiliza símbolos estándar para representar las operaciones lógicas.
2. Los diagramas de flujo son una representación gráfica de un algoritmo.
3. El pseudocódigo debe estar escrito en un lenguaje de programación específico.
4. Un diagrama de flujo siempre debe tener un inicio y un fin claramente definidos.

### Parte 5: Estructuras de Control

Describe para qué sirven las estructuras de control. Redacta dos ejemplos, uno de tu vida diaria, es decir cuando tienes que tomar decisiones en tus actividades diarias y oto ejemplo en el que se tengan que utilizar cálculos matemáticos para tomar una u otra decisión.

# Solución:

### Parte 1:

1. Una página web: No, porque una página web por sí sola no es como tal un algoritmo, ya que no describe una serie de pasos para resolver un problema. Puede contener algoritmos en su funcionamiento, pero la página en sí no lo es.
2. Una receta para hacer un pastel, donde se indican ingredientes y pasos a seguir: Si, es un algoritmo porque presenta una secuencia ordenada de instrucciones que, si se siguen correctamente, permiten obtener un resultado específico como lo es preparar un pastel.
3. "Piensa en un número y multiplícalo por otro": No, esta instrucción es muy general y no explica con claridad qué números utilizar ni cómo finalizar el proceso. Por eso no cumple con la característica de precisión de un algoritmo.
4. Un manual de instrucciones para armar un mueble, con pasos detallados y un orden claro: Si, es un algoritmo porque describe paso a paso el procedimiento para alcanzar un objetivo. Si se siguen las instrucciones en el orden indicado, siempre se obtiene el mismo resultado.
5. Una lista de compras organizada en orden alfabético: No, en una lista de compras solo contiene información organizada, pero no explica un procedimiento ni una secuencia de acciones para resolver un problema.

### Parte 2:

1. El valor de la gravedad en la Tierra (9.8 m/s²): Constante, porque su valor permanece fijo y no cambia durante la ejecución del algoritmo.
2. La edad de una persona: Variable, porque cambia con el paso del tiempo y depende de cada persona.
3. La cantidad de dinero en una cuenta bancaria: Variable, ya que puede aumentar o disminuir dependiendo de los movimientos realizados.
4. La velocidad de la luz en el vacío (299.792 458 m/s): Constante, porque es un valor fijo establecido por la física.
5. El radio de un círculo: Variable, porque puede tomar diferentes valores dependiendo del círculo que se esté analizando.

### Parte 3:

1. No cumple completamente, aunque busca encontrar la ruta más corta, utiliza la expresión "cuando los cambios parecen lo suficientemente pequeños", que es subjetiva y no define una condición exacta para terminar.
2. No cumple, la instrucción es demasiado general y no indica cómo se ingresan los números, cómo se realiza la suma ni cómo se muestra el resultado, por lo que no es precisa.
3. Sí cumple, el algoritmo tiene entradas definidas (base y altura), un proceso claro para calcular el área y una salida específica. Además, siempre produce el mismo resultado para los mismos datos.
4. Sí cumple, tiene un proceso bien definido para contar votos y una condición de finalización clara al ingresar el valor -1, por lo que es un algoritmo preciso y finito.

### Parte 4:

1. El pseudocódigo utiliza símbolos estándar para representar las operaciones lógicas, por lo cual es FALSO, el pseudocódigo se escribe utilizando lenguaje natural estructurado, mientras que los símbolos corresponden a los diagramas de flujo.
2. Los diagramas de flujo son una representación gráfica de un algoritmo, por lo cual es VERDADERO, utilizan símbolos y flechas para mostrar de manera visual el orden de ejecución de un algoritmo.
3. El pseudocódigo debe estar escrito en un lenguaje de programación específico, por lo cual es FALSO, el pseudocódigo es independiente de cualquier lenguaje de programación y solo sirve para describir la lógica del algoritmo.
4. Un diagrama de flujo siempre debe tener un inicio y un fin claramente definidos, por lo cual es VERDADERO, todo diagrama de flujo debe indicar dónde comienza y dónde termina el proceso.

### Parte 5:

Las estructuras de control sirven para organizar la ejecución de un algoritmo, estos permiten decidir qué instrucciones ejecutar y repetir procesos cuando sea necesario o seguir un orden determinado para resolver un problema de forma correcta y eficiente.

## Ejemplo de la vida diaria:

Cuando voy a salir de mi casa, primero reviso el clima, y si está lloviendo llevo un paraguas, de lo contrario, salgo normalmente. En este caso, la decisión depende de una condición.

## Ejemplo con cálculos matemáticos:

En un colegio se calcula el promedio final de un estudiante, y si el promedio es mayor o igual a 3.0, el estudiante aprueba la materia, si es menor a 3.0, la reprueba. Aquí la decisión se toma a partir de un cálculo matemático.


# Clase 11 de Agosto / 2026

# Taller de Algoritmos:

# Ejercicios con condicionales

### 1) **Control de temperatura del motor:**

- Durante una inspección de rutina, se mide la temperatura de un motor de turbina. Si la temperatura es mayor a un valor crítico, se debe indicar "Peligro: sobrecalentamiento". Si está dentro del rango seguro, indicar "Operación normal". Si es demasiado baja, indicar "Motor frío – Calentar antes de operar".

 ![Mi Imagen](https://github.com/Sebastian5050942/Toma_notas_Programaci-n/blob/4adbd03d59b7a603eac95d84a6191e2a2bf7f9c0/Ese6.drawio.png)

### 2) **Verificación de peso de despegue:**
    
- En una pista de pruebas de aeronaves, el sistema debe verificar si el peso total de la aeronave, incluyendo combustible y carga, supera el límite máximo permitido para el despegue. Dependiendo del resultado, el sistema deberá indicar si la aeronave está lista para despegar o si debe reducir carga o combustible.

 # Ejercicios de Bucles

### 1) Registro de altitudes de vuelo:
    
   Un sistema debe registrar la altitud de vuelo cada 10 minutos durante una hora y mostrar todas las mediciones al final.

   Inicio
   (Cont / Contador) = 0
   Leer nivel
   Mientras nivel ≥ max 0.1
         Cont = Cont + 1
         Leer nivel
   Fin - Mientras
Mostrar "Tiempo transcurrido" cont
Fin

### 2) Control de combustible en pruebas:
    
   Durante un ensayo en banco de un motor a reacción, se mide el nivel de combustible cada minuto y se detiene el registro cuando el combustible baja del 10%. Mostrar el tiempo total de operación antes de llegar a ese punto.


   Inicio
   Cont = 0
   Leer temp
   Mientras cont < 12
         Si temp > 27 o temp < 18
         Mostrar "Activar climatización"
      Fin si: cont = cont + 1
   Fin mientras
   Fin

   # Ejercicios de mayor complejidad

Durante la aproximación, un sistema recibe datos de altitud y velocidad cada 5 segundos hasta el aterrizaje. Si la velocidad excede el valor máximo seguro o la altitud no desciende adecuadamente, debe indicarse un mensaje de corrección de maniobra. Mostrar un resumen final de todos los avisos emitidos.

![Mi Imagen](https://github.com/Sebastian5050942/Toma_notas_Programaci-n/blob/ca9767c08a0b42728b3c8095b8cd8abe6548a8cc/Ese7.drawio.png)
