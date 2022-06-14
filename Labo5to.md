---
### Laboratorio de Programación Orientada a Objetos - Enunciados 
---

#### [Libro que utilizaremos en la materia](https://github.com/nadianoe/nadianoe.github.io/blob/master/labo/Luis%20Joyanes%20Aguilar_%20Ignacio%20Zahonero%20Mart%C3%ADnez%20-%20Programaci%C3%B3n%20en%20Java%20_%20algoritmos%2C%20programaci%C3%B3n%20orientada%20a%20objetos%20e%20interfaz%20gr%C3%A1fica%20de%20usuario-McGraw-Hill%20(2011)%20(1).pdf)

----

#### 14 de Junio

<details>
	<summary> Enunciado </summary>

```
- El trabajo consiste en implementar en Java un programa que será usado 
por una cadena de restaurantes. 

El programa deberá servir para:

*) Guardar un registro diario de los pedidos tomados por los mozos.
*) Consultar el número de mesas correspondiente a un plato.
*) Consultar el número de cada pedido.
*) Cuál fué el plato más pedido del día.
*) Cuál fué el plato menos pedido del día. 
*) Consultar el pedido que se debe entregar próximamente.
*) Cuál fué la mesa más ocupada en el día.

La cantidad de mesas variará pues si las mesas
posicionadas dentro del local están todas ocupadas y el clima lo permite,
se armarán nuevas mesas en la parte externa del local.

El restaurante ofrece una cantidad de 5 platos:

"Milanesa con puré de papas"
"Ravioles rellenos con carne"
"Pizza a la Piedra"
"Polenta con salsa Fileto"
"Arroz primavera" 

Tal lista variará pues puede suceder que todos los días se agreguen o 
quiten platos de la carta.

Cuando un cliente desocupa una mesa, la lista de pedidos asociada a la 
mesa se debe vaciar. No sucede con la lista de pedidos del restaurane 
pues se usará ésta información luego. Cuando un nuevo cliente ocupa una 
mesa, la lista de platos pedidos actuales se vuelve a llenar de nuevo.

Se deben proponer y programar las clases necesarias para cumplir con lo 
pedido. 

Utilizar al menos un HashMap, un HashSet y una lista.
```
</details>

-----

#### 8 de Junio

<details>
	<summary> Enunciado </summary>
	
- Con respecto al ejercicio del 10 de Mayo, ahora es necesario aumentar las funcionalidades del sistema propuesto.
- El sistema deberá:
1. registrar los tipos de tareas que ha decidido realizar: crear cuenta corriente, depositar dinero, extraer dinero.
2. permitir realizar las tareas mencionadas a través de un nombre de usuario, clave alfanumérica y DNI
3. consultar tanto el monto de dinero disponible como los datos de cada extracción o compra con la cuenta (cada
  movimiento bancario deberá estar acompañado de una fecha, una hora, una dirección (de cajero automático o comercio), 
  el monto extraído/depositado/consumido y una breve descripción de la operación realizada.
4. Deberá permitir generar un ticket/comprobante de la operación realizada indicando los datos del banco (nombre, dirección,
  CUIT, número de sucursal, número de caja (la caja podrá ser automática o atendida por una persona), los datos de la operación 
  y el saldo restante.
5. En el caso de las operaciones realizadas en cajas atendidas por personas, en el comprobante también se deberán agregar
  los datos del cajero que atendió al cliente.
6. Por último el sistema deberá permitir el nivel de satisfacción que tiene el cliente. 

- Recordar crear código de calidad: aplicar alta cohesión de métodos, colocar nombres declarativos y elegir estructuras de datos 
  adecuadas en cada situación aprovechando sus características.
	
</details>

-------

#### 7 de Junio

<details>
	<summary> Enunciado </summary>
	
- Realizar un sistema que controle la programación de una radio.

- Los horarios se controlan por bloques organizados de la siguiente manera:
	
```
00:00 hs a 6:00 hs	Bloque 1
6:00 hs a 9:00 hs	Bloque 2
9:00 hs a 13:00 hs	Bloque 3
13:00 hs a 17:00 hs	Bloque 4
17:00 hs a 20:00 hs	Bloque 5
20:00 hs a 00:00 hs	Bloque 6
```
	
- Todos los días se repite la misma distribución de bloques en la programación de la radio.

- Cada programa de radio tiene un nombre, horario (día y número de bloque) y una lista de conductores. Los conductores tendrán asociado un nombre, apellido y fecha de nacimiento.

- El sistema debe permitir la carga de conductores y programas de radio. Debe constatar que al asignar un horario al programa, el mismo no se superponga con otro. 

- Realizar las clases correspondientes con sus métodos asociados y un programa de prueba que demuestre el buen funcionamiento del sistema.
Adicionalmente, el programa de prueba debe mostrar por pantalla el listado de programas de un día elegido por el usuario.

</details>

------

#### 1 de Junio

<details> 
	<summary> Ejercicio 1 </summary>
	
```
Crear una mini-calculadora programable.
La calculadora se inicializa cargándole un programa.
Cada programa contiene varias rutinas y cada rutina está asociada a un nombre
y consta de una secuencia de instrucciones.
La calculadora opera con una pila que almacena valores numéricos, y 
con una memoria en la que se pueden guardar variables identificadas por nombre. 

Los programas pueden utilizar seis distintos tipos de operaciones: 
cuatro operaciones aritméticas (push, add, sub, mul), 
dos operaciones de manejo de variables (read, write).

Ejemplo:
La rutina "A" contiene las instrucciones:
	read(x)
	push(2)
	add
	write(y)

La Rutina "B" contiene las intstrucciones:
	push(2)
	read(x)
	mul
	write(x)
	
Operaciones aritméticas:

push(número), agrega una constante numérica en la pila.

add, saca dos valores del tope de la pila, los suma y apila el resultado. 
En caso de que la pila se encuentre vacía, se toma 0 como valor por defecto. En caso de que 
haya sólo un valor, se deja tal cual está.

sub, saca dos valores del tope de la pila, los resta y apila el resultado. 
El valor en el tope de la pila es el
sustraendo. Igual que para la suma, si la pila está vacía, el valor por defecto es 0.

mul, saca dos valores del tope de la pila, los multiplica y apila el resultado. 
Al igual que antes, si la pila está vacía, el valor por defecto es 0.


Operaciones de manejo de variables:

Las operaciones de manejo de variables permiten almacenar un valor en la memoria de 
la calculadora.

write(variable), saca el valor del tope de la pila y lo guarda en la variable indicada. 
Si la pila está vacía, el valor por defecto es 0.

ejemplo: 
	si la pila contiene sólo al valor 34
	las variables presentes en la memoria de la calculadora son
	x con valor 12 (en el tope)
	y con valor 45
	se ejecuta la instrucción write(x)
	entonces ahora la pila estará vacía porque el valor 34 se guardó
	en la variable x y la memoria pasará a tener los siguientes valores:
	x von valor 34 (en el tope)
	y con valor 45
											  
read(variable), mete en la pila el valor actual de la variable indicada. 
Si la variable no fue inicializada anteriormente, se considera que su valor 
por defecto es 0.

ejemplo: 
	si la pila se encuentra vacía
	las variables de la calculadora, tiene a: 
	x con valor 7 (en el tope)
    y con valor 32
	se ejecuta la instrucción read(y). Entonces, la pila
	ahora contendrá el valor 32.

-------------------------------------------------------------------

Cómo se utilizaría la calculadora?

Programa p = new Programa();

p.agregarInstruccion("rutinaA", new Instruccion("PUSH", 2));
p.agregarInstruccion("rutinaA", new Instruccion("ADD"));
p.agregarInstruccion("rutinaA", new Instruccion("WRITE", "y"));
p.agregarInstruccion("rutinaA", new Instruccion("READ", "x"));
p.agregarInstruccion("rutinaB", new Instruccion("READ", "x"));
p.agregarInstruccion("rutinaB", new Instruccion("MUL"));
p.agregarInstruccion("rutinaB", new Instruccion("WRITE", "x"));
p.agregarInstruccion("rutinaB", new Instruccion("PUSH", 2));

Calculadora calc = new Calculadora();
calc.cargarPrograma(p);
calc.ejecutar("rutinaB");
```
</details>


<details>
	<summary> Ejercicio 2 </summary>

Realizar un sistema que administre el consumo de electricidad de viviendas.

Cada vivienda tendrá a una dirección, si es un domicilio particular o una empresa y un dueño asignado. El dueño deberá tener asociado un nombre, un apellido y un DNI.

Una vez por mes se deberá cargar cuál fue el consumo de electricidad de cada vivienda. Al cargar el consumo se debe almacenar el mes y los KWh consumidos en ese periodo, comprobando que el mes no esté ya cargado para esa vivienda.

Se debe generar el método correspondiente para poder calcular lo que debe pagar cada vivienda por su consumo. Para dicho cálculo se utilizan dos valores:

1.	Para domicilios particulares: $2 el KWh
2.	Para empresas: $3 el KWh

Ejemplo: si una vivienda consumió en un mes 20KWh debe pagar $40.

Por otro lado si el consumo del mes se redujo un 10% respecto del consumo del mismo mes del año anterior se debe aplicar un descuento del 5% al número final.

Realizar las clases correspondientes con sus métodos asociados y un programa de prueba que demuestre el buen funcionamiento del sistema y cálculos ejemplo de lo que deben pagar las viviendas.

	
</details>

----

#### 24 de Mayo

<details> 
	<summary> Ejercicio </summary>
	
- Realizar un sistema que controle la asistencia de un empleado a su trabajo. 

El sistema será utilizado por una empresa con un nombre.
La empresa que lo utilizará cuenta con muchos empleados.
De cada empleado se conoce sus nombre, apellido, teléfono,
fecha de nacimiento, los nombres de sus días laborables, 
el horario laboral (hora de ingreso y egreso) y
los ingresos que realiza cada día (fecha y hora).

Se espera que el sistema permita obtener la siguiente 
información:

- el porcentaje de asistencia de un empleado
  en un determinado mes.
- la cantidad de empleados actuales
- el nombre, apellido y teléfono del empleado con una
asistencia del 100%
- el listado de nombres, apellidos y teléfonos de aquellos
empleados que tienen una asistencia menor al 50%
- el listado de nombres, apellidos y teléfonos de aquellos
empleados que llegan al menos 5 minutos tarde.
- la cantidad de empleados que deben trabajar por día
- la información el ítem anterior con forma de tabla

</details>

-----


#### 11 de Mayo

<details> 
	<summary> Enunciado </summary>

  - Realizar la conxión de java con una tabla de base de datos a elección. Se debrá lograr:
	- Realizar una inserción de 3 nuevas filas
	- Realizar dos actualización de dos datos distintos
	- Realizar una eliminación de fila
	- Realizar una selección de todos los datos de la tabla e imprirlos con el siguiente formato de ejemplo:
		- Nombre: Gloria - Apellido: "Rgofilis" - Edad: 89
		
</details>

<details>
	<summary> Bases de datos </summary>
	
- [Descargar .jar para realizar la conexión](https://github.com/materiasipm/materiasipm.github.io/raw/master/labo/octubre/mysql-connector-java-8.0.21.jar)

</details>
	
----

#### 10 de Mayo

<details>
	<summary> Enunciado </summary>
	
Se debe implementar una parte de un sistema que sirve para registrar las visitas de 
los clientes de un banco. Para ello, deberán:

- Crear la clase Persona, la misma debe tener como atributos: nombre y dni.
- Crear la clase Cliente, la misma debe tener como atributos: nombre, dni y cbu.
  
  Reutilizar la clase Persona teniendo en cuenta el concepto de herencia de clases.
- Crear la clase Banco, la misma deberá tener como atributos: nombre y una lista
  de clientes que visitaron al banco. 
  
  Esta clase deberá tener sólo el constructor por defecto.
- En la clase Banco, crear un método que retorne un HashSet que contenga los cbu's de
  los clientes que visitaron el banco. El método deberá llamarse "cbusDeClientesVisitantes".
- Crear un método que reciba un HashSet con la estructura del ítem anterior e imprima sus elementos.
- En la clase Banco, crear un método que retorne un HashMap cuyos pares clave-valor
  asocien el cbu de un cliente y la cantidad de visitas que realizó. 
  
  El método deberá llamarse "cantidadDeVisitasPorCliente"
- Crear un método que reciba un HashMap con la estructura del ítem anterior e imprima sus 
  elementos según el siguiente formato:
```
  clave: "121234343531" - valor: 3
```
	
</details>

<details>
	<summary> Ejercicio </summary>
	
- Crear una clase llamada Area (en inglés, sin tilde), esta clase deberá tener definidos
cinco métodos que sirvan para poder calcular el área de las siguientes
figuras geométricas:

	- Círculo. Fórmula para calcular el área: pi * radio * radio.
	- Esfera. Fórmula para calcular el área: 4 * pi * radio * radio.
	- Cuadrado. Fórmula para calcular el área: lado * lado.
	- Cubo. Fórmula para calcular el área: 6 * lado * lado.
	- Triangulo. Fórmula para calcular el área: base * altura / 2.

- Los método definidos deben ser estáticos y deben retornar el valor del cálculo
realizado. Utilizar la variable estática PI donde sea necesario.

	
</details>


----


#### 4 de Mayo

<details>
	<summary> Ejercicio 1 </summary>

Crear un sistema para administrar el saldo de la tarjeta de transporte llamada TarjetaEquis
y para llevar un registro de los pasajeros que están presentes en el medio de transporte.

El sistema consistirá en crear las clases

Clase Viaje, con atributos: precio, fecha, hora

(fecha y hora, por ahora, serán de tipo String)

Clase TarjetaEquis, con atributos: saldo, saldoNegativoMaximo, numeronId, lista "viajes"

La clase TarjetaEquis tendrá como métodos:
- "cargarSaldo(float monto)"
- "realizarViaje(Viaje viaje)"
- "ultimoMontoAbonado()"

Clase Pasajero, con atributos: nombre, apellido, tarjeta

Clase Sistema, con atributos: lista "pasajerosPresentes", lista "historialDePasajeros", línea 

La clase Sistema tendrá como métodos:
- "subePasajero(Pasajero pasajero, float monto)", método que no retorna nada; imprime "¡Bienvenido!"
en caso de que el usuario haya podido pagar su boleto exitosamente e imprime "Saldo Insuficiente"
en caso contrario.
- "seBajaPasajero(Pasajero pasajero)", método que no retorna nada
- "pasajerosQueSeHanSubidoAlgunaVez()", retorna una instancia de clase HashSet
- "pasajerosConUltimoMontoAbonado()", retorna una instancia de la clase HashMap
- "ultimoMontoAbonadoPorPasajero(float numeroId)", retorna el monto del pasajero que tiene la tarjeta con numeroId
   Utilizar el método "pasajerosConUltimoMontoAbonado()"

- Considerar el siguiente método y elegir en qué clase debería estar. Agregar parámetros
en caso que lo considere necesarios.
	- "seSuperaElSaldoNegativo()", método que retorna true en caso de superar el saldo negativo y 
	false en caso contrario

</details>
  
  ----

<details>
	<summary> Ejercicio 2 </summary>

1. Redefinir el método "toString()" de la clase Viaje, el string retornado deberá
contener los valores de cada atributo con el siguiente formato:
```
  hora: ... | fecha: ... | precio: ...
```
2.  Redefinir el método "toString()" de la clase Tarjeta, el string retornado deberá
contener la información de todos los viajes realizados según el siguiente formato:
```
  hora: ... | fecha: ... | precio: ... | saldo: ...
```
Utilizar el método "toString()" de la clase Viaje.

3. Redefinir el método "toString()" de la clase Pasajero, el string retornado deberá
contener la información del mismo según el siguiente formato:
```
  Nombre:
  Apellido:
  
  Viajes realizados:
  hora: ... | fecha: ... | precio: ... | saldo: ...
  hora: ... | fecha: ... | precio: ... | saldo: ...
  hora: ... | fecha: ... | precio: ... | saldo: ...
  hora: ... | fecha: ... | precio: ... | saldo: ...
  ...
  ...
  hora: ... | fecha: ... | precio: ... | saldo: ...
  hora: ... | fecha: ... | precio: ... | saldo: ...
```
Utilizar los métodos "toString()" de las clases Viaje y Tarjeta.

4. Aplicar el concepto de alta cohesión

</details>
	
----
	
#### 26 de Abril

<details> 
	<summary> Ejercicio  1 </summary>
	
- Con respecto al ejercicio relacionado con una librería, se necesitan agregar
funcionalidades. Ahora, no sólo administrará la cantidad de libros 
vendidos; también calculará el precio de libros comprados por cliente.

- Con respecto al precio de libros, la librería ofrece un cincuenta 
porciento de descuento al importe de cada libro que pertenece a cierto 
conjunto de editoriales.

Para ello, se debe:

- crear HashSet de editoriales con descuento en la clase Librería.

- crear un método que sirva para agregar editoriales al 
HashSet mencionado.

- Crear un hashmap para almacenar la información de cada venta realizada.
  Dicho hashmap debe asociar una instancia de la clase cliente con el importe total 
  de la compra que realizó.

- Deberá exitir una clase llamada Cliente que tendrá un id y un hashmap que
 asocia un libro y las unidades compradas del mismo.

- Las instancias de la clase Cliente deberán estar almacenadas en un hashset.

- Crear un método que imprima los libros comprados del cliente, sus respectivas
unidades y el importe total de la compra.	
</details>

<details>
	<summary> Ejercicio 2 </summary>

1) Crear una subclase de la clase persona que represente a un alumno de una escuela, debe llamarse Alumno. Los atributos que debe tener el alumno son:

- Curso, que debe ser de tipo String.
- Notas, que debe ser de tipo HashMap que asocia un String y un ArrayList de floats representando el nombre de la materia y las notas que tiene el alumno en la misma, respectivamente.
La declaración del atributo será la siguiente:
```java
  private HashMap<String,ArrayList<Float>> notasPorMateria;
```
2) Se deben crear los métodos:

- Agregar Nota
- Menor Nota
- Mayor Nota
- Promedio Notas

- Agregar Materia

Comentarios: 
- En el/los constructor/es de la clase Alumno sólo se deberán inicializar el HashMap
y el curso.
- El método agregarMateria se deberá declarar de la siguiente forma:
```java
  public void agregarMateria(String nombreDeMateria){
  
  }
```
 Y en la implementación, se deberá crear un ArrayList, inicializarlo y luego
 agregarlo al HashMap como valor acompañado de su correspondiente clave.

  </details>
	
	
----
	
#### 20 de Abril

<details> 
	<summary> Ejercicio </summary>
	
1. Crear un programa que le pida al usuario una cantidad
de números. La cantidad de números ingresados la determinará el usuario. Los números ingresados deberán ser guardados en un ArrayList.

- Luego, quitar los elementos repetidos del ArrayList utilizando
un HashSet; mostrar en pantalla los elementos que el ArrayList
contiene luego de haber quitado los repetidos.

2. Crear otro programa que le pida al usuario una cantidad
de números. La cantidad ingresada la determinará el usuario.
Los números ingresados deberán ser guardados en un ArrayList.

- Pedir que el usuario realice lo mismo otra vez, crear otro
ArrayList con los números ingresados en esta segunda vez.

- El programa deberá verificar si las dos secuencias tienen los 
mismos elementos, sin importar el orden o la cantidad de apariciones.
Utilizar la comparación de HashSets para realizar la verificación.

</details>

----

#### 13 de Abril

<details> 
	<summary> Exámen </summary>
	
1. Tomar la clase Persona creada en clases anteriores y agregarle 
	el método "esUnAdultoJoven" retorne true si la edad de la persona
	es mayor o igual a 18 y menor o igual a 35.

2. Crear la clase Canción que tenga como atributos: "nombre" (una variable de tipo String) y "duraciónEnSegundos" (una variable de tipo int)
   - Agregar un constructor por defecto y un constructor que reciba
   un nombre y una duración expresada en segundos.
   - Agregar un método que se llame "esUnaCancionLarga" que retorne
   true si la canción tiene una duración mayor o igual a 240 segundos.

3. Crear la clase Cantante como subclase de la clase Persona.
	- Agregarle el atributo "nombreArtístico" como variable de
	tipo String y el atributo "canciones" como variable
	de tipo ArrayList que sirva para almacenar objetos de la 
	clase Canción.
	- Agregar un método que se llame "obtenerCancionesMasLargas" 
	que retorne una lista con los nombres de las canciones más largas.
	- Agregar un método que se llame "agregarCanción" que reciba un nombre
	de canción y una duración en segundos.

4. Crear la clase SistemaDeCantantes que tenga como atributo una lista
   de objetos de la clase Cantante llamada "cantantes". 
   - Agregar un constructor por defecto.
   - Agregar un método llamado "obtenerCantantesJovenes" que retorne un
   ```ArrayList<Cantante>``` que contenga a los cantantes que tienen una edad entre 18 y 35. 
   - Agregar un método llamado "agregarCancion" que reciba tres parámetros: el nombre artístico del cantante, nombre de la canción y
   la duración de la canción en segundos. Este método deberá agregar una
   nueva canción a la lista de canciones del artista indicado.

5. Crear 1 objeto de la clase Cantante utilizando el constructor por 
   defecto y luego cambiarle el nombre artístico utilizando un "setter".
   Comprobar que el cambio se realizó correctamente utilizando un "getter".

	
	</details>
	
----
	
#### 6 de Abril

<details>
	<summary> Ejercicio </summary>
	
- Realizar un sistema para administrar pedidos de almuerzos realizados por alumnos.
- Para los alumnos además de los atributos de la clase Persona que ya tienen creada, se deberán incluir:
	- Curso
	- nro. de legajo
	- orientación
	
- Existen diferentes platos que se pueden solicitar, para ellos los datos a incluir son: Nombre y Precio.
	- Para esto, deberán crear la clase Plato y tener como atributos un nombre y un precio.
- Al cargarse un pedido se incluye la fecha de creación, el objeto Plato correspondiente, la persona que lo pidió, hora de entrega y si ya se entregó o no.
	- Para esto deberán crear la clase Pedido 
- Debe existir un menú (interfaz de usuario) donde se puedan agregar, modificar y eliminar pedidos. 
	- Estas funcionalidades deberán ser proporcionadas por una clase llamada "SistemaAlmuerzos".
- Se debe poder imprimir un listado de los platos a cocinar en el día con su precio considerando el descuento aplicado.
	- El método que realice ésto, deberá llamarse "imprimirInforme".
	
</details>


----

#### 30 de Marzo
  
<details>
	<summary> Enunciado </summary>

- Se debe implementar una parte de un sistema que sirve para registrar datos
de aquellos alumnos que salen y entran de sus aulas. Para ello, deberán:

- Crear la clase Persona, la misma debe tener como atributos: nombre y dni.
- Crear la clase Alumno, la misma debe tener como atributos: nombre, dni y nroDeLegajo.
- Crear la clase Aula, la misma deberá tener como atributos: número y una lista
  de alumnos que ingresaron a la misma durante todo un dia (si un alumno ya ingresó, salió
  y volvió a ingresar, se cuentan dos ingresos). Esta clase deberá tener sólo el constructor por defecto.
	
- En la clase Aula, crear un método que retorne un ArrayList que contenga los números de dni (sin repetidos) de los alumnos que ingresaron al aula durante el dia. El método deberá llamarse "dnisDeAlumnosIngresantes".

- Crear un método que reciba un ArrayList con la estructura del ítem anterior e imprima sus elementos.

- En la clase Aula, crear un método que reciba el dni de un alumno y
luego retorne la cantidad de ingresos que realizó. 

- En la clase Aula, crear un método que imprima por consola el dni de cada alumno y
la cantidad de ingresos que realizó. El método deberá llamarse "cantidadDeIngresosPorAlumno".
La impresión de sus elementos deberá respetar el siguiente formato:
```
  clave/dni: 121234343531 - valor/cantidad: 3
```
- Crear un método en la clase Aula que retorne el nombre del alumno que ha realizado más ingresos al aula.
	
</details>

----
#### 29 de Marzo
<details>
  <summary> Ejercicios </summary>
	
- Realizar los siguientes ejercicios del libro
  - página 220, ejercicio 8.1
  - página 266, ejercicio 10.7, 10.8
	
</details>

----
  
#### 22 de Marzo
  
<details>
  <summary> Enunciado </summary>
  
- Sea una librería, se necesita un sistema para administrar la información que 
se recolecta cada día.

- Actualmente, la librería vende libros de las siguientes editoriales:
	- Kapelusz, Sudamericana, Atlántida, ElAteneo, Interzona, Sur y Alianza.

- Editoriales con 50% de descuento:
	- ElAteneo, Interzona, Sur y Alianza.

Para ello, se deberá:

1. Crear la clase Libro, en la misma deben existir los atributos:
	- id
        - nombre
	- precio
	- editorial

2. Crear la clase Cliente, en la misma deben existir los atributos:
	- id
	- nombre
	- edad
	- libros comprados (ArrayList de libros)

3. Crear la clase SistemaLibreria, en la misma deben existir los atributos:
	- clientes (ArrayLis de clientes)
	- libros en venta (ArrayList de libros)
	- libros en oferta (ArrayList de id's)
	- libros vendidos (ArrayList de libros)
	- nombre

4. El sistema deberá tener métodos que permitan :
- obtener una lista de los clientes más frecuentes (se considera cliente frecuente al que
ha comprado más de 10 libros)
- obtener una lista con los libros más vendidos, es decir, aquellos libros
que han tenido más de 100 ventas
- obtener una lista con las edades de los clientes más frecuentes
- obtener una lista con los libros más caros, es decir, aquellos que salen más de $5500,50
- realizar una venta, es decir, crear una nueva instancia de la clase libro y agregarla
a la lista de libros vendidos
- obtener lista de los libros cuyos nombres comienzan con determinada letra 
- Calcular el precio final abonar por el cliente (tener en cuenta que los libros cuya editorial 
pertenece a las editoriales en oferta, tienen un 50% de escuento)
- cambiar el precio de un libro según el id. El porcentaje de descuento debrá ser
 pasado como parámetro.
- cambiar los precios por navidad:
	- si los id de los libros son pares, sus precios deberán disminuir un 25%
  - si sus id's son impares, sus precios deberán disminuir un 35%

#### Comentarios:
- No imprimir ni recibir datos por consola durante la clases pedidas. Piense y utilice los
parámetros que considere convenientes para sus métodos.
- Si desea probar sus funciones imprimiendo los resultados, deberá hacerlo dentro de una función "main".
Este método deberá estar dentro de la clase SistemaLibreria.
- Cada método deberá realizar una sola tarea
- Las clases deben comenzar con letra mayúscula
- los métodos ý variables deben comenzar con letra minúscula
- Utilizar el estilo de escritura camel case
- Utilizar nombres de métodos y variables declarativos
  
</details>

----

#### 16 de Marzo

<details>
  
<summary> Ejercicio - for each </summary>
  
- Crear una clase similar a la clase llamada "SistemaDeRegistro" realizada. Esta nueva clase sólo deberá utilizar 
  estructuras repetitivas de tipo "foreach". La nueva clase deberá llamarse "Sistema".

</details>

----
	
#### 9 de Marzo
  
<details>

<summary> Ejercicio 1 </summary>
  
- Crear una clase llamada Producto. La misma deberá tener como atributos:
    - nombre
    - precio

  El atributo nombre deberá ser de tipo String y el atributo precio
  deberá ser de tipo float.

  El programa deberá proveerle al usuario las siguientes tareas:

* Registro de producto.
  Aquí se deberá pedir el nombre del producto y su precio.

* Importe parcial a pagar.
  - Aquí se deberá imprimir el importe a pagar por 
  los productos registrados hasta el momento.
  - Cuando se termine de mostrar el importe mencionado, 
  el programa deberá dar la opción de realizar
  un nuevo registro.

* Finalizar registro. 
  Aquí se deberá imprimir el importe total a pagar.
  - Cuando se termine de mostrar el importe mencionado, 
  el programa no deberá dar la opción de realizar 
  un nuevo registro.
  
</details>

<details>

  <summary> Ejercicio 2 - ArrayList </summary>
  
  - Crear un sistema ABM. Un sistema ABM es un sistema que permite ralizar 3 acciones principales:
     - A -> alta -> ingreso de datos 
     - B -> baja -> eliminaciòn de datos
     - M -> modificaciòn -> modificación de datos

  - El ABM que realicen será un sistema que administre datos de personas.

  - Comentario: deberán utilizar la clase Persona que se pidió realizar la clase pasada.

  - Para ello, deberán:

1. Crear una clase que se llame "SistemaDeRegistroDePersonas". La misma deberá tener como
atriburo un arraylist que contenga objetos de la clase Personas. debe llamarse "personas".

2. El sistema deberá proveer 6 opciones que el usuario deberá elegir:

- Realizar el alta de una persona, es decir, registrar una persona. Crear un método que resuelva esta tarea.

- Realizar la baja de una persona, es decir, eliminar del registro a determinada persona. Crear otro método que resuelva esta tarea.
La eliminaciòn deberá hacerse segùn el nùmero de DNI. Crear otro método que resuelva esta tarea.

- Realizar alguna modificaciòn de algún/os dato/os una persona, es decir,brindar la opción
de modificar alguno de los atributos que tiene la persona. Crear otro método que resuelva esta tarea.

3. Tambièn le vamos a agregar funciones extra:

- Ver nombres de personas mayores de 18 años. Crear otro método que resuelva esta tarea.

- Ver lista de todas las personas registradas. Crear otro método que resuelva esta tarea.

4. También se deberá proveer la opción de Salir del sistema. 
El sistema deberá imprimir el mensaje "bye!"

</details>

----

#### 8 de Marzo

<details>
  <summary> Parte 1 </summary>
  
  1. Crear la clase Persona con los siguientes atributos:
  - nombre
  - edad
  - dni
  - telefono
  - dirección
    
  2. Declarar e implementar 3 tipos de constructores:
  - Uno por defecto.
  - Uno con parámetro string.
  - Otro con los 5 parámetros correspondientes a todos los atributos.
  - Declarar e implementar los getters y setters.

  3. Agregar métodos con los siguientes nombres:
  - esMayorDeEdad
  - sonLaMismaPersona
  - tienenLaMismaEdad
    
  
  - Dentro de la función main, crear 3 instancias distintasde la clase Persona. 
    A la primer instancia, cambiarle el valor de la edad por el doble de la misma.
    A la segunda instancia, cambiarle el valor del teléfono.
    Con respecto a la tercer instancia, imprimir por consola todos sus datos.
    
</details>
	
<details>
  <summary> Parte 2 </summary>
  
1. Crear una aplicación que pida al usuario ingresar los datos necesarios para crear un objeto de la clase Persona.
2. Crear la instancia de la clase Persona e imprimir cuáles fueron los datos ingresados utilizando "getters".
3. Ofrecerle al usuario la opción de cambiar uno de sus datos (el usuario deberá elegir), realizar el cambio utilizando
"setters" e imprimir nuevamente los datos del objeto creado.


</details>

  ------
  
