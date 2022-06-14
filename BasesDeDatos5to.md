---

## Bases de Datos - 5to

---

- Sitio web para generar datos aleatorios
	- [https://www.mockaroo.com](https://www.mockaroo.com/)
	
- Herramienta alternativa para ejecutar consultas de mysql
	- [https://paiza.io/en/languages/mysql](https://paiza.io/en/languages/mysql)

----

#### 27 de Mayo

- [enunciado parte 1](https://github.com/nadianoe/nadianoe.github.io/blob/main/examen27deMayoBD.pdf)

------

#### 20 de Mayo

<details>
  <summary> Enunciado </summary>
  
#### Trabajo práctico

- 2 integrantes

1. Buscar 3 data-sets a elección. Los tres data-sets deberán estar
relacionados en temática y deberán conformar una base de datos.
2. Crear una base de datos con datos con nombre declarativo.
3. Aplicar las 3 formas normales y realizar el diagrama entidad-relación de que represente la base de datos creada.
4. Transformar el data-set a inserciones SQL utilizando
herramientas online.
5. Proponer, escribir el enunciado y resolver 50 consultas que se puedan
realizar sobre la base de datos creada. Las consultas deberán
utilizar todos los temas vistos y presentar combinaciones.
6. Proponer, escribir el enunciado y resolver 50 stored procedures que se puedan realizar sobre la base de datos creada. Estos procedimientos
deberán utilizar estructuras condicionales, estructuras repetitivas
y todos los tipos de parámetros (in, inout, out) combinados entre sí.

- Comentario 
    - Deberán probar todas las consultas y stored procedures propuestos.

- Formato de entrega
  - El diagrama entidad relación y las respuestas de los puntos 5 y 6 deberán
    ser entregados de forma escrita a mano.
  - Los archivos .csv, el script .sql,
    y el código c++ (en caso de haber requerido utilizar) deberán ser entregados
    comprimidos por Teams.
  - Cada integrante deberá escribir 25 de las propuestas presentadas en los puntos 5 y 6

</details>

-------


#### 13 de Mayo

<details>
	<summary> Ejercicios </summary>
	
- Una empresa quiere llevar los datos de sus empleados, sus sueldos y las horas que trabaja como así  también los productos que venden sus Vendedores. Los empleados tienen un sueldo fijo mas las comisiones que sacan por ventas. Los empleados pueden ser de dos tipos administrativos (estos no tienen comisiones por ventas) y vendedores. 
Los datos que se necesitan son :

```
Empleados:
DNI
Apellido
Nombre
Domicilio
Sector 
Teléfono particular
Nro. De Interno 
Celular 
Estado Civil
Hijos  (puede aceptar valores nulos)
Fecha de nacimiento
Fecha de ingreso a la empresa

Sueldo:
Básico
Retenciones
Asignaciones
Comisiones
Mes
Sueldo Neto


Productos:
Descripción
Stock
Stock mínimo
Precio de Costo
Precio de venta
Demora en la entrega

Control de Horas:
Fecha
Hora de Inicio
Hora de fin

Productos vendidos por vendedores:
(Poner los campos necesarios)
```
	
MySql

1. Crear la base de datos y llamarla MiEmpresa.
2. Entrar en la base de datos.
3. Crear las tablas correspondientes.
4. Ingresar 5 registros en cada tabla.
5. Hacer un listado de los empleados que ingresaron en el año 1995.
6. Hacer un listado de los empleados que cumplen años en el mes de octubre. 
7. Hacer un listado de los empleados que cumplen años la primera quincena de enero.
8. Hacer un listado de la antigüedad de los empleados, expresada en años. Hay mas de una función que pueden utilizar en este caso planteen las alternativas que encuentren y elijan la mejor. 
9. Para los productos cuyo stock sea igual menor a su stock minimo hacer un listado de las fechas en las que se recibirá el producto si el pedido se hiciera hoy.
10. Hacer un listado que contenga el top ten de los empleados teniendo en cuenta los productos vendidos. Mostrar nombre y apellido de los empleados y cantidad de productos vendidos en lo que va del año.
11. Hacer un listado de los empleados y la cantidad de ventas durante el año 2017 agrupando por mes. El listados tendría que tener la siguiente información: nombre y apellido del empleado, año, mes, cantidad de productos vendidos.
12. Listar la desccripcion del producto y cantidad de vendidos por mes durante el 2017.
13. Que función utilizaría para convertir un string en un campo con formato de fecha valido, es decir un date. Muestre un ejemplo de su uso. 
14. Listado que contenga una columna llamada nombre_empleado con el siguiente formato: Apellido, nombre. Utilice la función apropiada y un alias.
15. Actualice la descripción de la tabla de productos, siempre que en la descripción de un producto se encuentre la palabra televisor reemplacela por la cadena TV. Utilice una función que le parezca apropiada.
16. Que función utilizaría para quitar espacios delante y atra de una cadena de caracteres. Inserte una fila con un dato que tenga espacios al inicio y al final; luego cree una consulta que elimine dichos espacios
utilizando la función propuesta. 
17. Haga un listado del nombre y apellido del empleado y la cantidad de hijos que tiene. Recuerde que el campo hijos puede contener null. El listado tiene que mostrar la cantidad de hijos o la leyenda NO TIENE si el campo tiene el valor null.
17. Hacer un listado que muestre la descripción del producto y una leyenda que diga MUY CARO, CARO, BARATO dependiendo del precio del producto según los siguientes rangos: menos de 3000 barato, entre 3000 y 6000 caro, mas de 6000 muy caro. Utilizar if.
18. Haga un listado que contenga nombre y apellido del empleado, sueldo neto y una leyenda que diga SUELDO ALTO, SUELDO MEDIO, SUELDO BAJO según el siguiente criterio: menos de 15000 BAJO, entre 15000 Y 50000 medio y  mas de 50000 ALTO. Utilizar case.
19. Hacer un listado de las fechas de ingreso de los empleados mostrando Nombre y Apellido, la fecha de ingreso con el siguiente formato Thursday 4th July 2013 y una cuarta columna con el dia de la semana en que se produjo dicho ingreso. Utilizar las funciones de fecha. 


</details>

-----

#### 6 de Mayo

<details>
	<summary> DER para resolver el ejercicio </summary>
	
- [DER](https://github.com/nadianoe/nadianoe.github.io/blob/main/classicmodels.pdf)
	
</details>

<details>
	<summary> Ejercicios </summary>

- [ejercicios](https://github.com/nadianoe/nadianoe.github.io/blob/master/bd5to2022/Ejercicios%20SP%20classicmodels.pdf)
	
</details>

-----

#### 29 de Abril

<details>
	<summary> Ejercicios </summary>

- Se pide aplicar normalizar hasta 3FN explicando el proceso de normalización, y  las decisiones tomadas para realizarlas. 

1. Una empresa de sistemas se dedica a desarrollar proyectos informáticos. Cada proyecto está asociado a una empresa cliente y en el pueden trabajar varios empleados. Se tienen los siguientes datos:

```
Código_proyecto
Nombre_proyecto
Horas_asociadas_proyecto
Codigo_empresa_cliente
Nombre_empresa_cliente
Dirección_empresa_cliente
Teléfono_empresa_cliente
Codigo_empleado
Nombre_empleado
Horas_empleado_proyecto
Dni_empleado
Categoría_proyecto
```

2.  Una empresa metalúrgica realiza distintos procesos como fundición, galvanizado, etc. Cada proceso esta asociado a un sector de la empresa y tiene varios insumos asociados al mismo. Se tienen los siguientes datos:

```
Código_proceso
Nombre_proceso
Horas_asociadas_proceso
Código_sector
Nombre_sector
jefe_sector
Teléfono_interno_sector
Código_insumo
Nombre_insumo
cantidad_utilizada_proceso
proveedor_insumo 
Categoría_insumo
```

3. En una empresa desarrolladora de juegos, cada juego es desarrollado por un sector de la empresa y cada sector esta compuesto por varios empleados. Se tienen los siguientes datos:

```
Código_juego
Nombre_juego
Descripción_juego
Código_sector
Nombre_sector
jefe_sector
Teléfono_interno_sector
Código_empleado
Nombre_empleado
horas_asignadas_empleado
dni_empleado
tipo_empleado
```

	
</details>

-----

#### 22 de Abril

<details>
	<summary> Enunciado </summary>
	
- Crear las consultas para las siguientes consultas 
según el DER presentado:

1. Seleccionar a todas las mascotas agrupadas por edad.
2. Seleccionar a todas las mascotas agrupadas por peso.
3. Seleccionar la cantidad de mascotas que hay según sus
edades. 
4. Seleccionar la cantidad de mascotas que hay según sus 
pesos.
5. Seleccionar la suma de los pesos de aquellas mascotas 
cuyas edades están entre los 5 y los 10 años.
6. Seleccionar el peso promedio de las mascotas.


- Stored Procedure

7. Crear un SP que reciba un id_amo y luego retorne la cantidad
de mascotas que tiene.
8. Crear un SP que reciba un id_mascota y luego muestre si la
mascota pesa más de 15 kg. 
9. Crear un SP que reciba un id_veterinario y luego imprima
todos sus datos
10. Crear un SP que reciba un número y luego muestre aquellas
mascotas que tienen un peso mayor o igual al indicado.
    - Invocar a este último SP pasándole el número 6 como parámetro.

```sql
	
-- SET GLOBAL sql_mode=(SELECT REPLACE(@@sql_mode,'ONLY_FULL_GROUP_BY',''));
-- SET sql_mode='STRICT_TRANS_TABLES,NO_ZERO_IN_DATE,NO_ZERO_DATE,ERROR_FOR_DIVISION_BY_ZERO,NO_ENGINE_SUBSTITUTION';
	
```

</details>

----

#### 8 de Abril

<details>
  <summary> Ejemplos vistos </summary>
  
```sql

DELIMITER $$
CREATE PROCEDURE incrementar(INOUT valor INT,IN incremento INT)
BEGIN
	SET valor = valor + incremento;
END$$


CREATE PROCEDURE prueba()
BEGIN
    DECLARE valor INT;
	SET valor = 1;
	CALL incrementar(valor,1); -- 2
	CALL incrementar(valor,1); -- 3
	CALL incrementar(valor,5); -- 8
	SELECT valor; -- 8
END$$

DELIMITER ;

CALL prueba();  

```
  
```sql
DELIMITER //

CREATE PROCEDURE es_positivo(IN numero INT)
BEGIN
    DECLARE respuesta BOOLEAN DEFAULT FALSE;
    IF (numero > 0) THEN
    	SET respuesta = TRUE;
    END IF;
    
    SELECT respuesta;
END //

DELIMITER ;

CALL es_positivo(12);
  
```
```sql
DELIMITER $$

CREATE PROCEDURE tipoDeNumero(IN valor_ingresado INT)
BEGIN
    DECLARE respuesta VARCHAR(100);
    IF (valor_ingresado > 0) THEN
    	SET respuesta = 'es mayor a 0';
    ELSEIF (valor_ingresado = 56) THEN
    	SET respuesta = "es igual a 0";
    ELSE 
    	SET respuesta = "es menor a 0";
    END IF;
    SELECT respuesta;
END $$

CALL tipoDeNumero(-1);
	
```

</details>


<details>
  <summary> Ejercicios </summary>

1. Crear un stored procedure que sirva para calcular el área de un rectángulo.
2. Crear un stored procedure que sirva para indicar si el número indicado es positivo y mayor a 100.
3. Crear un stored procedure que sirva para calcular el promedio de tres números recibidos como parámetros.
	
</details>

<details>
	<summary> Resoluciones vistas, propuestas y discutidas en clase </summary>
	
```sql

DELIMITER //

CREATE PROCEDURE calcular_area(IN base INT, IN altura INT)
BEGIN
	DECLARE area INT DEFAULT 0;
	SET area = base * altura;
	SELECT area;
END //


CREATE PROCEDURE es_positivo_y_mayor_a_cien_v1(IN valor INT)
BEGIN
	IF (valor > 0) THEN
		SELECT "Es positivo";
	END IF;
	IF (valor > 100) THEN
		SELECT "Es mayor a cien";
	END IF;
END //

-- otra forma

CREATE PROCEDURE es_positivo_y_mayor_a_cien_v2(IN valor INT)
BEGIN
	DECLARE es_el_buscado BOOLEAN;
	IF (valor > 100) THEN
		SET es_el_buscado = TRUE;
	ELSE
		SET es_el_buscado = FALSE;
	END IF;
END //

CREATE PROCEDURE promedio(IN valor1 INT, IN valor2 INT, IN valor3 INT)
BEGIN
	DECLARE promedio FLOAT;
	SET promedio = (valor1 + valor2 + valor3) / 3;
	SELECT promedio;
END //

DELIMITER ;

CALL calcular_area(5,8);
CALL es_positivo_y_mayor_a_cien_v1(101);
CALL es_positivo_y_mayor_a_cien_v2(101);
CALL promedio(2,1,3);

```
	
</details>

----

#### 1 de Abril

<details>
  <summary> Ejercicios - stored procedures </summary>
  
1. Crear un stored procedure que realice una consulta de todos los datos de las tablas clientes y productos.
2. Crear un stored procedure que reciba el número de cliente y luego se impriman sus datos.
3. Crear un stored procedure que muestre los datos de los clientes con un id mayor a 2 y hayan realizado al menos un pedido.
  
</details>

<details>
	<summary> Respuestas vistas en clase </summary>

- ejercicio 1

```sql
DELIMITER //

CREATE PROCEDURE obtenerDatosDeClientesYProductos()
BEGIN 
	SELECT * FROM clientes;
	SELECT * FROM productos;
END //
	
```
	
- ejercicio 2

```sql
DELIMITER //

CREATE PROCEDURE obtenerDatosDeCliente(IN id_cliente_i INT)
BEGIN 
	SELECT * FROM clientes WHERE id_cliente = id_cliente_i;
END //
```
	
- comentario y resolucion del ejercicio 3

```sql
CREATE DATABASE administracion;
USE administracion;

CREATE TABLE clientes(id_cliente int, nombre varchar(100));
INSERT INTO clientes (id_cliente,nombre) values 
	(1,"Olga"),(2,"Karina"),(3,"Julio"),(4,"Carlos"),(5,"Estela");

CREATE TABLE pedidos(id_pedido int, id_cliente int);
INSERT INTO pedidos (id_pedido,id_cliente) values 
	(1,1), (2,1),(3,2),(4,3),(5,3),(6,3),(7,4),(8,5);


SELECT id_cliente, COUNT(id_pedido) AS cantidad_de_pedidos 
FROM pedidos 
GROUP BY id_cliente
HAVING id_cliente > 2 AND cantidad_de_pedidos >= 1;


SELECT id_cliente FROM (
SELECT id_cliente, COUNT(id_pedido) AS cantidad_de_pedidos 
FROM pedidos 
GROUP BY id_cliente 
HAVING id_cliente > 2 AND cantidad_de_pedidos >= 1) AS ids_clientes;


SELECT * FROM clientes 
WHERE id_cliente 
IN(SELECT id_cliente FROM 
(SELECT id_cliente, COUNT(id_pedido) AS cantidad_de_pedidos FROM pedidos 
GROUP BY id_cliente HAVING id_cliente > 2 AND cantidad_de_pedidos >= 1) 
AS ids_clientes);
	

DELIMITER //

CREATE PROCEDURE obtenerClientesConIdMayorADos()
BEGIN
	SELECT * FROM clientes 
	WHERE id_cliente 
	IN(SELECT id_cliente FROM 
	(SELECT id_cliente, COUNT(id_pedido) AS cantidad_de_pedidos 
	FROM pedidos 
	GROUP BY id_cliente HAVING id_cliente > 2 AND cantidad_de_pedidos >= 1) 
	AS ids_clientes);
END //

	
/*
	Comentario: una forma alternativa de hacer esto es eliminando el "cantidad_de
	_pedidos >= 1" ya que si un cliente aparece en la tabla pedidos, dicho cliente
	realizó al menos un pedido.
*/
```
</details>
	
<details>
  <summary> Ejemplo sobre stored procedures </summary>
  
```sql
  
-- STORED PROCEDURES -- 

SELECT * FROM oficinas WHERE pais_o = pais;

DELIMITER //

CREATE PROCEDURE obtenerOficinas()
BEGIN
SELECT * FROM oficinas;
END //

DELIMITER ;
  
CALL obtenerOficinas();
  
DELIMITER //

CREATE PROCEDURE obtenerOficinasYEmpleados()
BEGIN
SELECT * FROM oficinas;
SELECT * FROM empleados;
END //

DELIMITER ;

CALL obtenerOficinasYEmpleados();

DELIMITER //
CREATE PROCEDURE obtenerOficinasPorPais(IN pais VARCHAR(255))
BEGIN
SELECT * FROM oficinas WHERE pais_o = pais;
END //

DELIMITER ;

CALL obtenerOficinasPorPais("Argentina");

DELIMITER $$

CREATE PROCEDURE CountOrderByStatus(IN orderStatus VARCHAR(25), OUT total INT)
BEGIN
   SELECT count(orderNumber)
   INTO total
   FROM orders
   WHERE status = orderStatus;
END$$

DELIMITER ;

```
</details>



<details>
  <summary> Ejercicios para realizar con subconsultas </summary>

Realizar las consultas sql apropiadas para responder a las siguientes preguntas: 

1) Listar para el cliente nro. 1 todos los pedidos realizados, indicando: el id, descripción, fecha de compra y fecha de entrega del pedido y los códigos de productos incluidos en el pedido.

2) Listar todos los pedidos de todos los clientes, indicando id cliente, nombre y apellido, id pedido y descripción de pedido.

3) Listar el detalle de los pedidos de los clientes. Incluir los siguientes datos en el listado: 
Del cliente: id, nombre, apellido.
Del pedido: id, descripción
Detalle del pedido: código de producto y cantidad.

4) Listar los clientes que aún no hayan realizado pedidos
  
5) eliminado

6) Listar el detalle de los pedidos cuyo descuento haya sido del 5%

7) Listar el/los pedidos con mayor descuento realizado

8) Listar el/los pedidos con menor descuento realizado

9) Listar los clientes que hayan realizado pedidos

10) Listar cuantos tipos de articulos se realizan por pedido

11) Listar los pedidos que que tengan mas de 3 articulos por pedido

12) Listar la cantidad de días desde la fecha de compra hasta la fecha de entrega por c/u de los pedidos

13) Listar los clientes con mas de 10 años de antigüedad

14) Listar para cada pedido el valor total de la compra

15) Listar los pedidos cuyo monto supere los $ 3500

16) Listar la cantidad de productos vendidos por codigo de producto

17) Listar el/los codigos de producto de mayor valor

18) Teniendo en cuenta el siguiente ejemplo:

|Nro de pedido	| Codigo de producto |	Cantidad |
|---------------|--------------------|-----------|
|1	| 1 |	2 |
|   |	5	| 5 |
|   |	7 |	3 |

El pedido nro 1 esta compuesto por 3 tipos de artículos diferentes y por 10 unidades en total teniendo en cuenta todos los productos. 

18.a.	Realice una consulta en la que se muestre la máxima, minima y promedio de unidades incluidas en un pedido.

19) Liste los nombres de los clientes que hayan realizado una compra por un valor total mayor a $3.000 

- respuesta ejercicio 11)

```sql
SELECT id_pedido,
(SELECT COUNT(*) FROM detallepedido WHERE detallepedido.id_pedido = pedidos.id_pedido) AS count 
FROM pedidos 
WHERE (SELECT COUNT(*) FROM detallepedido WHERE detallepedido.id_pedido = pedidos.id_pedido) > 3;
```

  
</details>

----
<details>
  <summary> 18 de Marzo - otro ejercicio de repaso </summary>
  
   - [DER y enunciado](https://github.com/nadianoe/nadianoe.github.io/blob/master/bd5to2022/ejercicio18deMarzo.pdf)
</details>

----

#### 18 de Marzo

<details>
  <summary> Archivos .sql para probar las soluciones propuestas </summary>
  
  - Descargar los scripts de la [siguiente carpeta](https://github.com/nadianoe/nadianoe.github.io/tree/master/bd5to2022)
    - pedidos.sql
    - detallespedidos.sql
    - clientes.sql
    - productos.sql
  - EJecutarlos y probar las soluciones propuestas para los ejercicios realizados la clase pasada.
</details>

----
- [11 de Marzo - ejercicio de repaso1](https://github.com/nadianoe/nadianoe.github.io/blob/master/bd5to2022/ejercicioSQL.pdf)
- [11 de Marzo - ejercicio de repaso2](https://github.com/nadianoe/nadianoe.github.io/blob/master/bd5to2022/ejercicios_parte2_11deMarzo.pdf)
