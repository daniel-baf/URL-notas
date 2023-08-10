La arquitectura Von Neumann es la base de la actualidad, la mayoria de las computadoras modernas están basadas en esta arquitectura, obviamente, no son iguales, solo lo usan de base.

## Origen

Antes, por ahí de los 1945, era muy común tener que recablear toda una computadora para poder hacer una tarea diferente, era tedioso y repetitivo.
En 1949 encontró y desarrolló la solución a este problema, que se basaba en poner la información sobre las operaciones a realizar en la misma memoria utilizada para los datos escribiéndola de la misma forma (código binario).

## Organización

Una computadora con esta arquitectura, consta de cinco partes
- Unidad aritmético lógico (ALU)
	- Circuito digital que realiza operaciones aritméticas (suma, resta) y operaciones lógicas (SI y NO)
	- Estos circuitos electricos por lo general están construidos dentro de los chips del microprocesador modernos.
	- ![Alu img](https://upload.wikimedia.org/wikipedia/commons/thumb/8/82/ALU_symbol.svg/1024px-ALU_symbol.svg.png)
- Unidad de control
	- Una de las principlaes unidades en las que se divide el CPU, su función es buscar las instrucciones en la memoria principal, decodificarlas (interpretarlas) y ejecutarlas, emplenado para ello la unidad de proceso.
	- ![img CU](https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fhardysoftwareg2sr.blogia.com%2Fupload%2F20110203023550-unidad-de-control.jpg&f=1&nofb=1&ipt=8d50da6ccb3d046eb17de757c42a47f3b59de764daca773713883602368fefdf&ipo=images)
- Memoria
	- Dispositivo que retiene, memoriza y almacena datos informáticos durante algún periodo de tiempo
	- ![img memoria informática](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse2.mm.bing.net%2Fth%3Fid%3DOIP.wJpBek-7fYoir8-lfQooDgHaFU%26pid%3DApi&f=1&ipt=5a8f0a7d54294ef3683d30ab16f48533458dc169c5bdacf5456e376410b6bc28&ipo=images)
- Dispositivo de entrada y salida
	- También conocidos como periférico, es el aparato o dispositivo auxiliar e independiente conectado a la computadora que permite la conexión de elementos externos al circuito de la computadora.
- Bus de datos
	- Este se usa como medio de transporte entre las distintas partes conectadas, también se le llama canal.
	- Formado por cables o pistas en un circuito impreso, con resistores y condensadores además de circuitos integrados.
	- Hay dos tipos de transferencia en los buses
		- Serie: transfiere datos bit a bit (monocanal)
		- Paralelo: transfiere varios bits simultaneamiente (multiples canales)
			- Aunque pareciera que la transferencia en paralelo es más eficiente, tiene inconvenientes. La frecuencia de reloj tiene que ser más reducida, y la longitud d elos cables de bus está ´limitado por posibles interferencias, ruido y retardos en la señal.
	- ![img buses](https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2F1.bp.blogspot.com%2F_HZEhKnCpTH0%2FTCtWy7gcozI%2FAAAAAAAAACM%2FlhwbKKPSBXM%2Fs1600%2Fbus.jpg&f=1&nofb=1&ipt=e7ce32c8966db7498407f072ab2de366e92271b7ab1ed09cd051029b91af2904&ipo=images)

Una computadora Von Neuman primero enciende la computadora y obtiene la sigueinte instruccińo desde la memoria en dirección indicada por el controlador de programa, luego aumenta el contador de programa en la longitud de instrucciones para apuntar a la siguiente, decodifica las instrucciones mediante la UC y ejecuta las instrucciones.

## Programa almacenado
Alan Turing, en su escrito "On Computable NUmbers, with an Application to the Entscheidung problem" desqueribe una máquina hipotética que llamó "máquina universal", y que ahora es conocida como "Máquina de Turing". Esta máquina tenía almacenamiento infinito (memoria en terminología actual) que contenía tanto las instrucciones como los datos.
Diseñar una máquina con programas almacenados era el objetivo de Von Neuman (EDVAC)
Un computador de prorama almacenado es el que almacena las intrucciones del programa en la memoria electrónica. Se pensó que un computador que en su diseño contenía un conjunto de instrucciones que podían ser almacenadas en memroia. El diseño de un programa almacenado también daba la posiblidad a los programas de ser modificacdos ellos mismos durante la ejecución, para ello, se necesitaba de un programa que incrementara o modificara las direcciones de memoria de algunas instrucciones, las cuales tenían que ser hechas manualmente en los primeros diseños.
Tratar instrucciones como datos es lo que hacen los ensambladores, compiladores y otras herramientas de programación automática.

Una de las cosa malas con la arquitectura Von N. es que el mal funcionamiento de un programa almacenado puede dañar el computador. La protección de la memoria y otras formas de control de acceso pueden ayudar a proteger contra modificaciones accidentales y/o maliciosas de un programa.

## Cuello de botella de Von Neumann

El canal entre el CPU y memoria genera un cuello de botella para el rendimiento del procesador. Cuando se quieren manejar grandes cantidades de datos, el CPU se ve obligado a esperar operaciones, la velocidad del procesamiento y cantidad d ememoria han aumentado más rápdio que el rendimiento en la transferencia entre ellos, así que continuamos agravando el problema.