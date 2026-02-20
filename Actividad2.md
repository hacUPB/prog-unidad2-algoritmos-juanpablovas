# Actividad 2: Representación de Algoritmos

## **Conceptos importantes**

### Operadores Relacionales
En la mayoria de los casos utilizamos los siguientes operadores relacionales:  
- Igual a =  
- Mayor que >  
- Mayor o igual ≥  
- Menor que <  
- Menor o igual ≤  
- Diferente ≠ 

### Bucles
- For: El bucle for se utiliza cuando se conoce de antemano la cantidad de iteraciones, especificando un inicio, una condición y un incremento o decremento.  

- While: El bucle while ejecuta el bloque de código mientras la condición sea verdadera, siendo útil cuando no se conoce el número exacto de iteraciones.

- Do while: garantiza que el bloque de código se ejecute al menos una vez, ya que evalúa la condición al final de cada iteración.



## **Ejercicio 1**
Investiga cuáles son los símbolos que se utilizan para representar cada operación de un algoritmo con un diagrama de flujo. 

### Solución
En clase se establecieron los siguientes simbolos para emplear en un diagrama de flujo:  

*Inicio / Final:* Se utiliza para establecer el inicio de un diagrama de flujo con un elipsoide y al mismo tiempo, en el mismo diagrama, se finaliza el flujo del algoritmo con la misma figura geométrica.  
  
![alt text](Imagenes/SimboloStart.jpg)  

*Acción / proceso:* Representa una acción o instrucción general que debe realizarse. Se representa con un rectángulo.  

![alt text](Imagenes/Acción.jpg)  

*Decisión:* Muestra una operación condicional de formar booleana. Se representa con un rombo.  

![alt text](Imagenes/Decision.jpg)  

*Entrada:* Es una forma de ingresar o leer datos de entrada. Se representa con un paralelogramo.  

![alt text](Imagenes/entrada.jpg)  

*Linea de flujo:* Muestra el orden del algoritmo o de operación de los procesos, siguiendo una lógica.    

![alt text](Imagenes/LineadeFlujo.jpg)

*Muestra / Impresión:* Indica el proceso de imprimir o mostrar una variable de salida.

![alt text](Imagenes/Muestra.jpg)

## **Ejercicio 2**
Construye un algoritmo que, al recibir como datos el ID del empleado y los seis primeros sueldos del año, calcule el ingreso total semestral y el promedio mensual, e imprima el ID del empleado, el ingreso total y el promedio mensual.
### Solución
Análisis

 |Variable de entrada|Descripción|
 |- |-|
 |ID |Identificación del empleado| 
 |S1, S2, S3, S4, S5, S6 |Ingreso de cada mes|

 |Variable de salida|Descripción|
 |- |-|
 |X |Ingreso total semestral| 
 |Y |Promedio mensual|
    
    Inicio
        Leer ID, S1, S2, S3, S4, S5, S6  
        X = S1+S2+S3+S4+S5+S6  
        Y = X/6  
        Mostrar ID, X ,Y  
    Fin

## **Ejercicio 3**
Un acuario necesita determinar cuántos litros o galones (eso lo decide el usuario) de agua caben en un acuario, pero solo dispone de una cinta métrica (en centímetros). Diseña un algoritmo para solucionar el problema. 

### Solución
Análisis

 |Variable de entrada|Descripción|
 |- |-|
 |X, Y, Z |Ancho, largo y alto (cm)| 
 |N|Unidad seleccionada|

 |Variable de operación|Descripción|
 |- |-|
 |V |calculo de volumen en $cm^{3}$ |

 |Variable de salida|Descripción|
 |- |-|
 |M |Volumen en unidad seleccionada|        

    Inicio
        Mostrar: "Ingresa el ancho, el largo y el alto del acuario"
        Leer X, Y ,Z 

        Mostrar: "Si deseas conocer el volumen en litros digita 1, si quieres en galones digita 2" 
        Leer N

        M = 0

        V = X*Y*Z 

        Si N = 1
            Entonces
            M = V / 1000
            Mostar: "La capacidad en litros es" M

            Si no
            M = V / 3785.41
            Mostar: "La capacidad en galones es" M
        Fin si
    Fin

## **Ejercicio 4**
Realice un algoritmo para determinar cuánto se debe pagar por equis cantidad de lápices considerando que si son 1000 o más el costo es de $85 cada uno; de lo contrario, el precio es de $90. Represéntelo con el pseudocódigo y el diagrama de flujo.

### Solución
Análisis

 |Variable de entrada|Descripción|
 |- |-|
 |X |Cantidad de Lápices| 

 |Variable de salida|Descripción|
 |- |-|
 |V |Valor a pagar| 
    
    Inicio
        Mostrar: "Cuantos lápices deseas llevar el día de hoy"
        Leer X

        Si X >= 1000
            Entonces
            V = X*85

            Si no
            V = X*90
        Fin si
        Mostrar: "El valor de la compra es:" V
    Fin

## **Ejercicio 5**
Un almacén de ropa tiene una promoción: por compras superiores a $250 000 se les aplicará un descuento de 15%, de caso contrario, sólo se aplicará un 8% de descuento. Realice un algoritmo para determinar el precio final que debe pagar una persona por comprar en dicho almacén y de cuánto es el descuento que obtendrá. Represéntelo mediante el pseudocódigo y el diagrama de flujo.

### Solución
Análisis

 |Variable de entrada|Descripción|
 |- |-|
 |X |Valor de compra| 

 |Variable de salida|Descripción|
 |- |-|
 |V |Valor a pagar| 
    
    Inicio
        Mostrar: "Cuanto es el valor de tu compra"
        Leer X

        Si X > 250000
            Entonces
            V = X*0.15

            Si no
            V = X*0.08
        Fin si
        Mostrar: "El valor de la compra es:" V
    Fin

## **Ejercicio 6**
El director de una escuela está organizando un viaje de estudios, y requiere determinar cuánto debe cobrar a cada alumno y cuánto debe pagar a la compañía de viajes por el servicio. La forma de cobrar es la siguiente: si son 100 alumnos o más, el costo por cada alumno es de $65.00; de 50 a 99 alumnos, el costo es de $70.00, de 30 a 49, de $95.00, y si son menos de 30, el costo de la renta del autobús es de $4000.00, sin importar el número de alumnos.

### Solución
Análisis

 |Variable de entrada|Descripción|
 |- |-|
 |X |Cantidad de alumnos| 

 |Variable de salida|Descripción|
 |- |-|
 |M |Valor a pagar por estudiante| 
 |V |Valor total pagado por los estudiantes|
    
    Inicio
        Mostrar: "Cuantos estudiantes irán de viajes"
        Leer X
        M = 0
        V = 0

        Si X >= 100
            Entonces
            M = 65
            V = X*M

        Si no
            Si X >=50
                Entonces
                M = 70
                V = X*M

            Si no
                Si X >=30
                    Entonces
                    M = 95
                    V = X*M

                Si no 
                    V = 4000
                    
                Fin si
            Fin si
        Fin si
        Mostrar: "El valor de la compra a pagar en la compañia de viajes es:" V "Y se debe cobrar a cada alumno:" M
    Fin

## Evaluación: Compresión de Conceptos

### Parte 1: Identificar Algoritmos
Responde si los siguientes enunciados representan un algoritmo. Justifica la respuesta:

- Una página web: *Una página web no es una secuencia como tal de pasos a seguir.*  

- Una receta para hacer un pastel, donde se indican ingredientes y pasos a seguir. *Si podría ser un algoritmo, si los pasos y las instrucciones son claras.*  

- "Piensa en un número y multiplícalo por otro". *No especifica como se procesa ni como se muestra, además no intenta solucionar un problema o no tiene un objetivo claro.*  

- Un manual de instrucciones para armar un mueble, con pasos detallados y un orden claro. *Si sería un algoritmo, pero no debe tener ambiguedades.*

- Una lista de compras organizada en orden alfabético *Una lista de compras no tiene una finalidad como tal y mucho menos es una secuencia de pasos.*

### Parte 2: Variables y Constantes

Indica si las siguientes afirmaciones describen una variable o una constante:

- El valor de la gravedad en la Tierra, 9.8 m/s² (Constante)
- La edad de una persona calculada con base en el año actual y su año de nacimiento. (Variable)
- La cantidad de dinero en una cuenta bancaria. (Variable)
- La velocidad de la luz en el vacío, 299,792,458 m/s. (Constante)
- El radio de un círculo. (Variable)

### Parte 3: Características de los Algoritmos

Responde si los siguientes enunciados cumplen con las características de un algoritmo. Justifica la respuesta:

1. Para elegir la ruta más corta entre varias ciudades, el algoritmo examina rutas candidatas, deteniéndose cuando los cambios en la distancia parecen lo suficientemente pequeños.(No es objetivo, no termina con un objetivo y no es preciso)
2. Suma los números ingresados y muestra el resultado.(Le puede faltar un poco precisión, ¿cómo se van a ingresar los datos?)
3. Un conjunto de pasos para calcular el área de un rectángulo dado su base y altura. (Si los pasos están precisos, es deterministas y finito)
4. El algoritmo cuenta el número de votos obtenidos por cada uno de los candidatos de una elección para presidente. Empieza solicitando el nombre del candidato y finaliza cuando se ingresa el valor -1. (Si)


### Parte 4: Comprensión de Herramientas

Indica si las siguientes afirmaciones son ciertas o falsas respecto al pseudocódigo y diagramas de flujo:

1. El pseudocódigo utiliza símbolos estándar para representar las operaciones lógicas. (Falso)
2. Los diagramas de flujo son una representación gráfica de un algoritmo. (Verdadero)
3. El pseudocódigo debe estar escrito en un lenguaje de programación específico. (Falso)
4. Un diagrama de flujo siempre debe tener un inicio y un fin claramente definidos. (Verdadero, y en general un algoritmo)

### Parte 5: Estructuras de Control

Describe para qué sirven las estructuras de control. Redacta dos ejemplos, uno de tu vida diaria, es decir cuando tienes que tomar decisiones en tus actividades diarias y oto ejemplo en el que se tengan que utilizar cálculos matemáticos para tomar una u otra decisión.  

Las estructuras de control sirven para dirigir el flujo de ejecución de un programa. Permiten que el computador tome decisiones, repita acciones o ejecute instrucciones en un orden específico según se cumplan ciertas condiciones.

Ejemplos:
- Me estoy preparando para salir a la universidad. Si está lloviendo, entonces llevo paraguas. Si no, salgo normalmente sin paraguas.  

- Tengo tres notas: 3.5, 4.0 y 2.8.
    Prom = $\frac{3.5 + 4.0 + 2.8}{3} = 3.43$  
Si el promedio es mayor o igual a 3.0, entonces apruebo.
Si no, repruebo.





