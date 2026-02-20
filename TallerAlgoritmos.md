# Taller de Algoritmos

## **Enunciados de los problemas**

### **Ejercicios con condicionales**

1. **Verificación de peso de despegue**
    
    En una pista de pruebas de aeronaves, el sistema debe verificar si el peso total de la aeronave, incluyendo combustible y carga, supera el límite máximo permitido para el despegue. Dependiendo del resultado, el sistema deberá indicar si la aeronave está lista para despegar o si debe reducir carga o combustible.

Análisis

**Pseudocodigo**

 |Variable de entrada|Descripción|
 |- |-|
 |P |Peso limite| 
 |A |Peso aeronave| 

    Inicio
        Mostrar: “Ingresa el peso límite de despegue de la aeronave”
	    Leer P
        Mostrar: “Ingresa el peso de la aeronave”
        Leer A

        Si A > P
	        Mostrar: “Reducir carga o combustible”
        Si no
	        Mostrar: “Aeronave lista para despegar”
        Fin si
    Fin
**Diagrama de flujo**  

![alt text](Imagenes/Diagram1.jpg)

--- 
2. **Control de temperatura del motor**
    
    Durante una inspección de rutina, se mide la temperatura de un motor de turbina. Si la temperatura es mayor a un valor crítico, se debe indicar "Peligro: sobrecalentamiento". Si está dentro del rango seguro, indicar "Operación normal". Si es demasiado baja, indicar "Motor frío – Calentar antes de operar".

Analisis

**Pseudocodigo** 

 |Variable de entrada|Descripción|
 |- |-|
 |P |Peso limite| 
 |A |Peso aeronave| 

    Inicio
        Leer T
        Mostrar: Ingresa valor critico
        Leer X
        Mostrar: Ingresa valor motor frio
        Leer Y

        Si T >=X
	        Mostrar: “Peligro. Sobrecalentamiento”
        Sino
	        Si T<=Y
	            Mostrar: “Motor frío – Calentar antes de operar
	        Si no
	            Mostrar “Operación normal”
	        Fin si
        Fin si
    Fin

---

### **Ejercicios con bucles**

1. **Registro de altitudes de vuelo**
    
    Un sistema debe registrar la altitud de vuelo cada 10 minutos durante una hora y mostrar todas las mediciones al final.

Analisis

**Pseudocodigo** 

 |Variable de entrada|Descripción|
 |- |-|
 |H |Altitud| 
 |U |contador| 

    Inicio
        C = 0
        Mientras C <= 60
            Leer H
            C = C + 10
        Fin mientras
    Mostrar H 
    Fin

---
    
2. **Control de combustible en pruebas**
    
    Durante un ensayo en banco de un motor a reacción, se mide el nivel de combustible cada minuto y se detiene el registro cuando el combustible baja del 10%. Mostrar el tiempo total de operación antes de llegar a ese punto.
    
        Inicio
            C = 0  
	        Leer L  
	         X = L  
	        Mientras X > 0.1L  
		        Leer N  
		        C = C+1  
		        X=X-N  
	        Fin mientras  
	        Mostrar C
        Fin      
    
---

### **Ejercicios con bucle y condicionales**

1. **Detección de turbulencia en trayecto**
    
    Un sensor mide la aceleración vertical de la aeronave en intervalos de un segundo durante un trayecto de 2 minutos. Si el valor medido supera un umbral, indicar que se ha detectado turbulencia en ese instante. Al final, mostrar cuántas turbulencias se detectaron.

        Inicio
            Mostrar: “Ingresa el umbral de turbulencia”
            Leer U
            X=0

            Desde C = 1 hasta C = 120
	        Leer V
	        Si V > U
		        Mostrar: “Turbulencia”
		        X=X+1
	        Fin si
            Mostrar X
        Fin


  ---  
2. **Control de temperatura en cabina**
    
    Un sistema mide cada 5 minutos la temperatura en cabina durante una hora. Si en algún momento se detecta una temperatura mayor a 27°C o menor a 18°C, debe indicar que se active el sistema de climatización.

        Inicio
            C = 0
            Mientras C <= 12
            Mostrar: Ingresa temperatura en cabina
            Leer T

            Si T > 27
                Mostrar: Activar sistema de climatización
            Sino
                Si T < 18
                    Mostrar: Activar sistema de climatización
                 Sino
                    Mostrar: Temperatura dentro del rango normal
                Fin si
            Fin si

            C = C + 1

            Fin mientras
        Fin
    ---
    
3. **Simulación de conteo de pasajeros**
    
    Durante el abordaje, un sistema cuenta a los pasajeros que ingresan. Si el número total supera la capacidad máxima, el sistema debe detener el conteo y mostrar un mensaje de alerta.

    C = Pasajeros  
    W = Capacidad de la aeronave  
    X = Sensor en puerta  

        IniciO
            C = 0
            Mostrar: Ingrese capacidad maxima
            Leer W

            Mientras C <= W
                Leer X
                C = C + X

                Si C > W
                    Mostrar: Alerta. Capacidad maxima superada
                Fin si

            Fin mientras
        Fin
    

---

### **Ejercicios de mayor complejidad**

1. **Planificación de misión satelital**
    
    Desarrollar un algoritmo que reciba datos de consumo de energía por hora de un satélite durante un día completo. Si en cualquier hora el consumo excede un límite crítico, debe registrarse como una alerta. Al final, mostrar el consumo total y el número de alertas generadas.

    C = Consumo de energia  
    L = Limite critico  
    i = Contador de horas  
    j = Contador de alertas  
    x = Almacenamiento de consumo

        Inicio
            Mostrar: Ingresa el limite critico
            Leer L
            i = 0
            j = 0
            X = 0

            Mientras i <= 24

                Leer C
                X = X+C

                Si C > L
                    Mostrar "Alerta"
                    j = j +1
                Fin si

                i = i + 1

            Fin mientras
        Fin

---
    
2. **Simulación de carga y balanceo de aeronave**
    
    Una aeronave tiene varias bodegas de carga. El sistema debe permitir ingresar el peso cargado en cada bodega y verificar que:
    
    - El peso total no exceda el máximo permitido.
    - Ninguna bodega individual supere su límite.
        
        Mostrar mensajes de advertencia si alguna condición no se cumple. 

        i → Entero (contador de bodegas)

        n → Entero (cantidad de bodegas)

        p → Real (peso ingresado por bodega)

        t → Real (peso total acumulado)

        m → Real (peso máximo total permitido)

        l → Real (límite máximo por bodega)

        Inicio
        
            t = 0
            i = 0

            Mostrar: Ingrese numero de bodegas
            Leer n
            Mostrar: Ingrese peso maximo total permitido
            Leer m
            Mostrar: Ingrese limite maximo por bodega
            Leer l

            Mientras i < n
                Mostrar: Ingrese peso de la bodega
                Leer p

                Si p > l
                     Mostrar: Advertencia. Bodega supera limite individual
                Fin si

                t = t + p
                i = i + 1
            Fin mientras

            Si t > m
            Mostrar: Advertencia. Peso total excede maximo permitido
            Fin si

            Mostrar: Peso total cargado es: , t
        Fin
    

---
        
3. **Monitoreo de aproximación a pista**
    
    Durante la aproximación, un sistema recibe datos de altitud y velocidad cada 5 segundos hasta el aterrizaje. Si la velocidad excede el valor máximo seguro o la altitud no desciende adecuadamente, debe indicarse un mensaje de corrección de maniobra. Mostrar un resumen final de todos los avisos emitidos.

    c → Entero (contador de lecturas)

    a → Real (altitud actual)

    b → Real (altitud anterior)

    v → Real (velocidad actual)

    m → Real (velocidad máxima segura)

    r → Entero (contador de avisos)

        Inicio
            c = 0
            r = 0

            Mostrar: Ingrese velocidad maxima segura
            Leer m
            Mostrar: Ingrese altitud inicial
            Leer b

            Mientras b > 0
                Mostrar: Ingrese nueva altitud
                Leer a
                Mostrar: Ingrese velocidad actual
                Leer v

                Si v > m
                     Mostrar: Correccion de maniobra. Velocidad excesiva
                    r = r + 1
                Sino
                    Si a >= b
                    Mostrar: Correccion de maniobra. Altitud no desciende
                    r = r + 1
                    Fin si
                Fin si

                b = a
                c = c + 1
        Fin mientras

        Mostrar: Total de avisos emitidos: , r
    Fin