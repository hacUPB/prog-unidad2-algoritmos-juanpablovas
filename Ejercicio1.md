# Conceptos
### Datos en el mundo digital

- **Enteros:** se representan en binario.  

- **Reales:** Se representan mediante la notación de (IEEE 754) que consta de de 32 bits dividos en:
  - signo (1bit)
  - Exponente (8bits - Byte)
  - Mantisa (23 bits)  

- **Caracteres:**
    - ASCII: Cada caracter se representa con un número decimal entre 0 y 255, que se pueden representar luego en binario.  
    
      Aqui tenemos el codigo ASCII:  

      Imagen ()
    - Unicode: Nos permite representar más simbolos y alfabetos

- **Imágenes:** Se presentan por medio de matrices de píxeles, representados por valores numéricos (colores RGB). Los colores se pueden representar en sistema Hexagesimal, HTML, entre otros.

- **Sonidos:** Son muestras numéricas de la señal de audio.

### Almacenamiento Digital de Datos

- **Unidades de almacenamiento:**
  - 1 byte = 8 bits
  - 1 KB = 1024 bytes
  - 1 MB = 1024 KB
  - 1 GB = 1024 MB
  - 1 TB = 1024 GB

- **Sistema Hexadecimal**
Es un sistema en base 16 empleado para representar datos binarios de forma mas compacta

|Decimal|Hexadecimal|Binario|
 |- |-|-|
 |10 |A|1010|
 |15 |F|1111|


# Ejercicios 

## Ejercicio 1
### ¿Cuántos estados diferentes se pueden representar usando  N bits?

Con un solo bit se tienen 2 posibles estados, que son 0 ó 1. De esta manera, siguiendo la secuencia si se tienen 2 bits, se tienen cuatro posibles estados. 

De esta forma.

 |Bits|Estados|
 |- |-|
 |1 |2|
 |2 |4|
 |3 |8|
 |...|...|
 |N |$2^{N}$|

## Ejercicios

### 1. Convierte el numero decimal 22 a binario.

 **Solución:**

 22 = 16 + 4 + 2  
 22 = $2^{4}$ + $2^{2}$ + $2^{1}$


 |16|8|4|2|1|
 |- |-|-|-|-|
 |1 |0|1|1|0|

 ### 2. ¿Cuál es el resultado en decimal del número binario 10110?

 **Solucion:** 
|$2^{5}$|$2^{4}$|$2^{3}$|$2^{2}$|$2^{1}$|$2^{0}$|
|-|-|-|-|-|-|
|32|16|8|4|2|1|
|-|-|-|-|-|-|
|0|1|0|1|1|0|

10110 = $2^{4}$ + $2^{2}$ + $2^{1}$

10110 = 16 + 4 + 2

**10110 = 22**

## Ejercicios 2

### 1. ¿Qué número binario representa el carácter 'C' en ASCII? 

En el codigo ASCII la letra "C", se representa con el numero 67:

C = 67

|$2^{6}$|$2^{5}$|$2^{4}$|$2^{3}$|$2^{2}$|$2^{1}$|$2^{0}$|
|-|-|-|-|-|-|-|
|64|32|16|8|4|2|1|
|-|-|-|-|-|-|-|
|1|0|0|0|0|1|1|

C = 1000011

### 2. Convierte el número flotante 5.75 a binario (explica los pasos).

Paso 1: Se separa el 5

|$2^{3}$|$2^{2}$|$2^{1}$|$2^{0}$|
|-|-|-|-|
|8|4|2|1|
|-|-|-|-|
|0|1|0|1|

5= 101

Paso 2: Se separa el 0.75 y se multiplica por dos

0.75 * 2 = 1.5 (1)
0.5 * 2 = 1 (1)

5,75 = 101.11

## Ejercicios 3

### 1. ¿Cuántos bytes se necesitan para almacenar la palabra “Hola” en ASCII?

H = 1001000  
O = 1001111  
L = 1001100  
A = 1000001  

HOLA = 1001000 1001111 1001100 1000001

HOLA = 28 Bits
HOLA = 3.5 Bytes

Pero teniendo en cuenta que por una sola letra se puede emplear un byte, para almacenar la palabra se pueden utilizar 32 bits o 4 bytes

## Ejercicios 4

### Convierte el número decimal 255 a hexadecimal.

Decimal = 255

Binario 

|$2^{8}$|$2^{7}$|$2^{6}$|$2^{5}$|$2^{4}$|$2^{3}$|$2^{2}$|$2^{1}$|$2^{0}$|
|-|-|-|-|-|-|-|-|-|
|256|128|64|32|16|8|4|2|1|
|-|-|-|-|-|-|-|-|-|
|0|1|1|1|1|1|1|1|1|

255 = 1111 1111  
255 = FF

## Ejercicios Finales

1. Explica, en tus propias palabras, por qué es necesario que las computadoras representen los datos en binario.

2. Convierte el número binario 10011011 a decimal y a hexadecimal.

3. Investiga y describe cómo se representa una imagen en formato PNG en el disco.

4. Analiza la siguiente situación: ¿Qué sucede si intentas almacenar un número mayor al que puede representar un byte (por ejemplo, 300)? ¿Cómo lo maneja Python?

    
