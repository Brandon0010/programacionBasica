# programacionBasica

----
### Tutorial de Python.

###Operadores

TIPOS DE DATOS BASICOS

En python los tipos de datos básicos se dividen en, números, como pueden ser 3 (entero ó integer) 1.75, (punto flotante ó float) 7+5j (complejos ó complex).

Para poder conocer el tipo de dato de una variable susaremos la instrucción "type()".

Otro tipo de dato basico en PYTHON son las cadenas de texto, por ejemplo, "Hola Mundo" (cadena de texto o string ó 'Hola Mundo' ó "Jenny's dog").

Como se puede notar a diferencia de muchos otros lenguajes en PYTHON no se declara el tipo de variable al crearla.

Para resumir en PYTHON se puede reprecentar números enteros, reales, y complejos. Los números enteros son aquellos números positívos o negatívos que no tienen desimales. En la mayor parte de las maquinas las variables enteras ("int") pueden almacrnar números de -2^31 a 2^31. En plataformas de 64 bites el rango es de -2^63 a 2^63.
Operadores:

		suma                    r=3+2
		resta	                r=4-7
            (guión) negación        r=-7
		multiplicación		r=2*6
		exponente		r=2**6
		división		r=3.5/2
		división entera		r=3.5//2
		modulo (residuo)	r=7%2

Un ejemplo de esto puede ser el siguiente:

    a=int(input('Incerta un numero '))   
    b=int(input('Incerta otro numero '))

    s=a+b   
    print('La suma es ' ,s)    
    r=b-a   
    print('La resta es ' ,r)    
    m=a*b   
    print('El producto es ' ,m)   
    d=a/b   
    print('El residuo es ' ,d)   
    dd=b/a
    print('El resultado es ' ,dd)    
    p=a**b   
    print('El resultado de "a" a la "b" es ' ,p)   
    import math    
    print('El logaritmo es ' ,math.log10(a))

###Ciclo For.

En pyhton "for" se utiliza como una forma genérica de interés sobre una secuencia, es decir, recorrer una secuencia.

            variable = secuencia  
            secuencia = ["uno", "dos", "tres"]  //estos son elementos
            for elemento in secuencia:
                print(elemento)                //4 esopacios 

Y los resultados serán:

           uno
           dos
           tres
    
El ciclo "for" debe marcarse con un rango como se muestra de la siguiente manera:

    for temperatura in range(0,100,10):    //range es el rango y va el inicio, hasta
                                             donde quiero llegar y en este caso va de 10
    print(temperatura,'gC')                  en 10.

Un ejemplo del ciclo "for" puede ser el siguiente:

    for celcius in range(0,101,10):
        farenheit = (1.8*celcius)+32
        print(celcius,'gC','|',farenheit,'gF')

###Modulo Turlte 

Hay muchos módulos en python que proveen características poderosas que podemos usar en nuestros propios programas. Algunos de estos pueden enviar correos electrónicos y algunos de estos pueden extraer información de paginas de Internet. Para el manejo de gráficos usaremos un modulo que permite crear figuras y patrones. El modulo que se usara permiten desarrollar nuestro pensamiento computacional.

      
    import turtle
    ventana=turtle.Screen()	//Crea una ventana en blanco			
    alex=turtle.Turtle()	//Crear un objeto de la clase turtle lo puedo llamar como yo quiera se llama "alex" y puede tener atributos
    alex.forward(50)	//Avanza 50 unidades
    alex.left(90)		//gira a la izquierda 90°
    alex.forward(30)	//Avanza 30 unidades
    ventana.mainloop()	//Hasta que el usuario cierra la ventana el programa termina

Un ejemplo del modulo Turtle puede ser:

     import turtle
     ventana=turtle.Screen()
     alex=turtle.Turtle()
     alex.forward(100)
     alex.left(90)
     alex.forward(100)
     alex.left(90)
     alex.forward(100)
     alex.left(90)
     alex.forward(100)
     alex.left(90)
     alex.forward(100)
     ventana.mainloop()

Te aparecera una flecha, y no como tal una tortuga, pero si la quisieras ponlo de la siguiente manera:

    import turtle
    ventana=turtle.Screen()
    ventana.bgcolor('red')
    ventana.title("Hola")

    alex=turtle.Turtle()
    alex.shape("turtle")
    alex.color("blue")
    alex.pensize(10)
    alex.forward(100)
    alex.left(120)
    alex.forward(100)
    ventana.mainloop() 

###Funciónes 

Una función es un fragmento de código con un nombre asociado que realiza una serie de tareas y devuelve un valor. A demás de ayudarnos a programar y depurar dividiendo el programa en partes, las funciones también permiten reutilizar código.
     
	##definicion de una funcion
	def ladra():
	    print('guau, guau')
	##cuerpo principal del programa
	ladra()
Las Funciones ayudan al programador a dividir un problema en pequeñas piezas que pueden ser re usadas. También ayudan al programador a concentrarse en una pequeña parte del programa a la vez. Como resultado el escribir funciones es una parte importante del desarrollo del sofware. 

En nuestro caso debemos aprender a:

	1. Definir una función para usarla después.
	2. Pasar uno o más valores a una función.
	3. Desarrollar un cálculo complejo en una función.
	4. Regresar uno o más resultados a una función.
	5. Llamar a una función que previamente hayamos definido.

Puede también colocarce el Modulo Turtle con algunos de los ciclos, como se muestra este, con Ciclo For:

    import turtle
    def dibujar_cuadro(tur, d):
        for i in range(4):
            tur.forward(d)
            tur.left(90)
    ventana=turtle.Screen()
    ventana.bgcolor('green')
    ventana.title('Funciones')
    rafa = turtle.Turtle()
    dona = turtle.Turtle()
    dibujar_cuadro(rafa, 50)
    dibujar_cuadro(dona, 200)
    ventana.mainloop()

###Programación Ambientada a Objetos.

Al principio del curso comentavamos que Python es un lenguaje multiparadigma en el que se podía trabajar con programación estructurada, como veniamos haciendo ahora o con programación orientada a objetos el cual es un paradigma de programación en el que los conceptos del mundo real relevantes para nuestro problema se modelan a travéz de clases y objetos, y en el que nuestro programa consiste en una serie de interacciones entre objetos.

>OBJETOS:

>Un objetos es una entidad que agrupa un estado y una funcionalidad relacionada. El estado del objeto se define a través de variables llamadas atributos, mientras que la funcionalidad de modela a través de funciones a las que se les conoce con el nombre de MÉTODOS DEL OBJETOS.

>**Diagrama UML sirve para definir un objeto y culales son su métodos y sus atributos**

>Un ejemplo de objeto podría ser un coche en el que tendriamos Atributos como: la marca, el numero de puertas, o el color.

>Y Métodos como: arrancar, parar.

>O bien cualquier otra combinación de Atributos y Métodos según lo que fuera relevante para nuestro programa.

>CLASES:

>Una clase no es más que una plantilla genérica de la cual insancia los objetos; es la plantilla que define que Atributos y Métodos tendrán los objetos de esa clase.

En PYTHON las clases de definen Mediante la palabra clave "CLASS" seguido del nombre de la clase, seguido por dos puntos, y a continicación, inentado el cuerpo de la clase.

Por ejemplo:

    class Coche(object):
        def __init__(self,gasolina):
            self.gasolina = gasolina
        def arrancar(self):
            if self.gasolina > 0:
                print('Arranca')
            else:
                print('No Arranca')
        def conducir(self):
            if self.gasolina > 0:
                self.gasolina = self.gasolina - 1
                print('Quedan ', self.gasolina,' litros')
            else:
                print('No se mueve')
    vocho = Coche(5)
    tsuru = Coche(3)

    vocho.arrancar()
    vocho.conducir()
    vocho.conducir()
    vocho.conducir()
    vocho.conducir()
    vocho.conducir()

#UNIDAD 1

###Introducción a los ejercicios de programación

Los ejercicios estas diseñados para desarrollar en el alumno(a) la oportunidad de practicar problemas pequeños en pasos secuenciales. Adicionalmente se volverá familiar la sintaxis de Python, desarrollando los siguientes temas: 


* Generar una salida con la sentencia Print

* Leer la entrada del usuario con el teclado usando raw_imput

* Realizar cálculos sencillos con suma +, resta -, multiplicación 
*, división / ó //, modulo %, y potencia ** 

* Realizar cálculos más complejos con el modulo math 


* Para entrar a la terminal, escribir el comando Python para salir de 
* Python usamos exit. 

Existen dos formas de ejecutar código en Python, la cual puede ser mediante una sesión interactiva (línea a línea) con el intérprete o bien de la forma habitual, escribiendo el código en un archivo de código fuente y ejecutando. En la primera parte de este curso lo haremos con el intérprete.
El primer programa que vamos a escribir en Python, es el clásico “Hola mundo”, y en este lenguaje es tan simple como:


    Print (‘Hola mundo’)
    Comando  Argumentos (cadena de texto)

    mi_cadena = Tengo hambre y faltan 60 min. Para salir

    Variable Valor

Un comentario en Python inicia con el carácter reservado # 

>Ejercicio 1.

Crear un programa que despliegue su nombre y su dirección, tal y como lo vería en un sobre de una “cuenta”.

>Ejemplo.

    José Pérez Rodríguez

    Av. Mav Mediterraneo 222, Col Popotla, CDMX, CP:04032 

>>> Python
>>> Nombre = Brandon Acxel Romero Rivas
>>> Direccion = Calle Ignacio Zaragoza, No. 21, Col Loma Colorada 1 secc. Naucalpan de Juarez, CP. 53420
>>> Print (Nombre) 
>>> Print \ n
>>> Print (Direccion)
>>> Exit.

“python interviews” expo de 2 personas …. Resumen obtención y eso… Kenneth reitz Mike Driscoll
Documentos (bloc/notas) “.py”                           doc, archivos, etc. Insertar un programa / archivo …. “dir”  dc dirección el nombre comenzando con “python nombre.py”                         input

Escribir un programa que le pregunte al usuario por su nombre. El programa debe responder con un mensaje de “hola” + nombre del usuario.

    
    BLOC DE NOTAS

    Print (‘inserta tu nombre’)

    Nombre = imput ( )

    Print (‘hola + nombre’)

Escribe un programa que le pregunte al usuario el largo y el ancho de su cuarto de su habitación. Una vez que los valores han sido leidos el programa debe calcular y desplegar el área de la habitación. El largo y el ancho deben ser convertidos a números flotantes. Que incluya las unidades en su mensaje de salida.

Variable de tipo flotante: Es una variable que puede guardar datos numéricos con punto decimal. Para forzar a una variable o que sea flotante. “Float ( )”         Entero a decimal  -  “int ( )”     Decimal a entero

Ejercicio 4          

#####ÁREA DE UN CAMPO

Escriba un programa que le pida al usuario el largo y el ancho de un campo de futbol. Se debe de imprimir después el área del campo a cres.

>TIP : Un acre tiene 43,560 ft² = 0.000247105 acre.

    NOTAS
    Print (‘Inserta el largo del campo de futbol:’)
    Largo = input ( ) 
    Print (‘ Inserta el ancho del campo de futbol: ‘)
    Ancho = input ( )
    Área = largo * ancho
    Print (‘el área del campo de futbol es : ‘, área)


>EJERCICIO PYTHON TAREA 1.py

Inserta el largo del campo de futbol:
450 ft

Inserta el ancho del campo de futbol:
700 ft

El área del campo de futbol es: 
31500 ft²

>EJERCICIO 5

En algunos lugares, un deposito pequeño es agregado a los contenedores de basura, para hacer que las personas reciclen botellas de PET.
Actualmente el municipio paga $1 peso si se deposita una botella de PET vacía de un litro o menos y $2.50 pesos si se deposita una botella de PET vacia de mas de 1lt. Escriba un programa que le pregunte al usuario por el numero de botellas de 1 lt o menos, por mas numero de botellas de mas de un litro y que despliega al final, cuanto se le va a pagar al usuario por haber reciclado las botellas.

>EJERCICIO 6

El programa que usted va a escribir para este ejercicio comienza leyendo el costo de una comida ordenada en un restaurante. Después el programa debe calcular el impuesto (16%) y la propina (10%) por la comida. La salida debe incluir el costo de la comida, el impuesto, la propina y el total que debe pagar el usuario. Formatee la salida de los números para que estos aparezcan con el símbolo de pesos y con dos decimales. La salida debe de parecerse a un ticket del restaurant por lo que puede inventar el nombre del restaurante y la dirección.

>**Tipos de datos básicos 

Python y tipo de datos básicos se dividen en números, como pueden ser 3 (centeno o interger), 1.75 (de punto flotante o float) o bien 7+5; (complejos o complex).
Para poder conocer el tipo de dato de una variable usaremos la instrucción type ( ).
Otro tipo de dato básico son cadenas de texto por ejemplo 

* “Hola mundo”
* ‘Hola mundo’
* “Jeny´s day”

Como se puede notar a diferencia de muchos otros lenguajes, en Python no se declara el tipo de variable al crearlo.
Para resumir en Python se pueden representar en números enteros, reales y complejos. Los números enteros son aquellos números positivos o negativos que no tienen números decimales. En la mayor parte de las maquinas las variables enteros (int) pueden almacenar números de -2³¹ a 2³¹. En plataformas de 64 bits el rango es de -2⁶³ a 2⁶³. Los números flotantes son los que tienen decimales. En Python se expresan mediante el tipo “float”.
Se pueden representar de -2⁶⁴ hasta 2⁶⁴
Los números complejos son aquellos que tienen una parte imaginaria. Para definir una variable compleja se utiliza el termino complex.

###OPERADORES

###Operadores aritméticos

    Operador	     Descripción               Ejemplo  	 Resultado

    +                     Suma                     r = 3+2            5
    -	              Resta                    r = 4-7	         -3
    -	              Negación                 r = -7	         -7
    *	              Multiplicación           r = 2*6	         12
    **	              Exponente                r =2**6	         64
    /	              División	               r = 3.5/2	  1.75
    //	              División entera          r = 3.5//2	  1.0
    %	              Modulo	               r =7%2	          1

EJERCICIO 10     

####Números aritméticos

Escriba un programa que lea dos números enteros y los guarde en las variables “a” y “b”. El programa debe calcular y mostrar:

1. La suma de “a y b”
2. La resta de “b menos a”
3. El producto de “a y b”
4. El cociente cuando “a” es dividido por “b” 
5. El residuo de cuando “a” es dividido por “b”
6. El resultado de “aᵇ”
7. Resultado de log base 10 de ᵃ log10ᵃ 

>Comando log10 del modulo math

#UNIDAD 2

##Control de Flujo

###Sentencias condicionales

   Si un programa no fuera más que una lista de órdenes a ejecutar de forma secuencial, una por una, no tendría mucha utilidad. Los condicionales nos permiten comprobar condiciones y hacer que nuestro programa se comporte de una forma u otra que ejecute un fragmento de código u otro, dependiendo de esta condición.
 Aquí es donde cobran su importancia del tipo booleano y los operadores lógicos. 
Condicional “if”.
La forma más simple de una sentencia condicional es el “if” (del ingles si) seguido de la condición a evaluar “(:)” dos puntos, y en la siguiente línea el indentado, en código a ejecutar en caso de que se cumpla dicha condición. 

    Condicional if     Comprobaciones
    if	        Comprobación o condición                                              ¿a = B?             a - = b
    4 espacios forzosos # Código a ejecutar en caso de que la condición sea verdadera.  ¿a no es igual a b?    a! = b                                        
    ¿a es mayor a igual ab?	a >= b
    ¿a es menor a igual ab?	a < = b
>Variante if ….. else

>Mantener dos resultados

if comparación 1:

    # Código de la comparación 1

elif comparación 2:

    # Código de la comparación 2

elif comparación 3:
    
    # Código de la comparación 3

else
    
    # En caso de que las comparaciones de arriba no sean ciertas


Sentencias if     Import     numpy     as     np
    
               Import matplotlib.pyplot as plt
               # creando un vector numérico
               x = np.arange (100)
               y = np.sin(x) 
               #graficando
               plt.plot(x,y)
               plt.show( )

##BUCLES

Mientras que los condicionales permiten ejecutar distintos fragmentos de código dependiendo de ciertas condiciones, los bucles permiten ejecutar un mismo fragmento de código un cierto número de veces mientras se cumpla una determinada condición.

###WHILE

El bucle “while” (mientras) ejecuta un fragmento de código mientras se cumpla la condición.
El bucle while tiene la siguiente estructura.

*While condición:

    Fragmento de código que se repite

En Python “for” se utiliza como una forma genérica de interar sobre una secuencia, es decir, recorrer una secuencia

Ciclo for ….. in

    print (elemento)

    Elementos
    Secuencia = [“uno”, “dos”, “tres”]
    For elemento in secuencia 

Escriba un programa que despliegue una tabla de conversión de temperaturas para Celsius y grados Farenheit.

La tabla debe contener filas para todas las temperaturas desde 0 hasta 100° Celsius en múltiplos de 10°C.

Una tienda de descuento esta ofreciendo el 60% de descuento en productos descontinuados, la tienda quiere ayudar a los clientes con una tabla impresa pegada en los anaqueles que muestre el precio, el descuento que se va a aplicar y el precio original.

Escribe un programa que realice esa tabla con los siguientes precios originales.

    Precio original	     descuento	    Precio final

    4.95	                60%	

    9.95		

    14.95		
    
    19.95		

    24.95		

    199.5		

#####Funciones

Una función es un fragmento de código con un nombre asociado que realiza una serie de tareas y devuelve un valor. Además de ayudarnos a programar y deporar dividiendo el programa en partes, las funciones también permiten reutilizar código.

Las funciones ayudan al programador a dividir un problema en pequeñas piezas que pueden ser reusadas. También ayudan al programador a concentrarse en una parte del programa a la vez. Como resultado el escribir funciones es una parte importante del desarrollo del software. En nuestro caso debemos aprender a: 

* Definir una función para usarlo después 

* Pasar una o más valores a una función

* Desarrollar un cálculo complejo en una función

* Regresar uno o más resultados en una función 

* Llamar a una función que previamente hallamos definido

En la ciudad de México, la tarifa de uber tiene una base de 7.25 pesos, más 7 pesos por cada km recorrido.

Escribe una función que tome la distancia viajada (en km) y regrese el total que debe pagar el usuario. Tenga en cuenta que la tarifa mínima a pagar es de 40 pesos.

Hay módulos en Python que proveen características poderosas que podemos usar en nuestros programas. Algunos de estos pueden enviar correos electrónicos y algunos extraer información de páginas de internet para el manejo de graficos usaremos un modulo que permite crear figuras sin patrones. El modulo que se usara permite desarrollar nuestro pensamiento computacional.

Modificar el programa anterior para que antes de crear la ventana se le pregunte al usuario que color de fondo desea, debe guardar la respuesta en una variable y modificar el color del fondo de la ventana de acuerdo a los deseos del usuario.

El programa debe preguntarle al usuario cuantos círculos quiere.

* Código: import turtle 

    1. Ventana = turtle.Screen ( )
       Ventana.setup (500,500)
       Ventana.tracer (0)
       Ventana.addshape (“nombre.gif”)


    2. Mario = turtle.Turtle ( )
       Mario.speed (0)
       Mario.shape (“mario.gif”)


    3. Mario.penop ( )
       Mario.goto (-350,0)


    4. While true:
       Ventana.update
       Mario.forward (0.01)


* Programa: hacer que el objeto se detenga

###Programación orientada a objetos

Al principio del curso comentábamos que Python es un lenguaje multiparadigma en el que se podía trabajar con programación estructurada, como veníamos haciendo hasta ahora o con programación orientada hasta objeto el cual es un paradigma de programación en el que los conceptos del mundo real, relevantes para nuestro problema se modelan a través de clases y objetos, y en el que nuestro programa consiste en una serie de interacciones de nuestro sistema.




###Clases y objetos

Un objeto es una cantidad que agrupa un estado y una funcionalidad relacionada. El estado del objeto se define a través de variables llamadas atributos, mientras que la funcionalidad se modela a través de funciones a las que se les conoce con el nombre de métodos del objeto.

Un ejemplo de objeto podría ser un coche en el que tendríamos atributos como marca, No. de puertas, o el color y método de “arrancar y parar” o bien cualquier otra combinación de atributos y medios, según lo que fuera relevante para nuestro programa.

###Clases

Una clase no es más que una plantilla genérica de la cual instancia los objetos, es la plantilla que define que atributos y métodos tendrán los objetos de esa clase.

En Python las clases se definen mediante la palabra clave “class” seguido del nombre de la clase seguido de dos puntos “ : ” y a continuación identado el cuerpo de la clase.

    Class Automovil:

    Ejemplo      def…. init _ _ (self, atributo 1)

                 self.atributo 1 : atributo 1

                 Defarrancar (self) :

                 Método


    Cancion     Feliz_cumple = canción ( [“Letra”] ) 

    Feliz_cumple.cantame_una_cancion

    * Letra (str)
    * Cantante_una_canción ( )

Hacer una función que dibuje un cuadro de tamaño  d  usando el módulo turtle

range ( 4 ) ---> [0, 1, 2, 3]

 r = 2
