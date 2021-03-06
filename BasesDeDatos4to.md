#### 10 de Junio

<details>
  <summary> Ejemplos vistos </summary>
  
```sql
  
SELECT * FROM alumnos
WHERE NOT edad = 12;

SELECT * FROM alumnos WHERE nombre LIKE 'a%';

SELECT * FROM alumnos WHERE nombre LIKE '%a';

SELECT * FROM alumnos WHERE nombre LIKE '%a%';

SELECT * FROM alumnos WHERE nombre LIKE 'g%a';

SELECT * FROM alumnos
ORDER BY edad;

SELECT * FROM alumnos
ORDER BY edad DESC;

SELECT * FROM alumnos
ORDER BY nombre;
                                                                                       
SELECT * FROM alumnos
ORDER BY nombre DESC;
                                                                                       
SELECT *
FROM alumnos
WHERE edad IS NULL; 

SELECT *
FROM alumnos
WHERE edad IS NOT NULL; 
                                                                                 
UPDATE alumnos
SET nombre = "Alfredo", edad = 12
WHERE id = 1;
                                                                                       
UPDATE alumnos
SET nombre = "Alfredo", edad = 12
WHERE id IS NULL;                                                                                    

SELECT * FROM alumnos
LIMIT 3; 

SELECT * FROM alumnos
WHERE edad > 12
LIMIT 3; 
  
CREATE TABLE mascotas (
  id     INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
  nombre VARCHAR(100) NOT NULL,
  edad   INT NOT NULL,
  genero VARCHAR(50) NOT NULL
);

create table usuarios (
  nombre varchar(20),
  clave varchar(10),
  primary key(nombre)
 );

INSERT INTO mascotas (nombre, edad, genero)
VALUES
  ("Pepo",5,"macho"),
  ("Lolo",2,"hembra");

ALTER TABLE personas
ADD dni INT; 

ALTER TABLE personas
DROP COLUMN dni; 

ALTER TABLE productos
ADD precio INT; 

SELECT * FROM productos
WHERE nombre LIKE '%o%';

SELECT * FROM productos
WHERE nombre LIKE '%o%r%'; -- 

FLOAT
-- con .

ALTER TABLE productos
MODIFY COLUMN precio FLOAT; 

DATE 
-- YYYY-MM-DD
-- "2022-03-01"

DATETIME 
-- YYYY-MM-DD HH:MI:SS

SELECT MIN(precio)
FROM productos;

SELECT MIN(precio)
FROM productos WHERE id >= 10 ;

SELECT MAX(precio)
FROM productos;

SELECT COUNT(precio)
FROM productos
WHERE condicion;

SELECT AVG(precio)
FROM productos
WHERE condicion;  

SELECT SUM(precio)
FROM productos
WHERE condicion; 

ALTER TABLE productos CHANGE precio precioUnitario FLOAT;

SELECT precio
FROM productos
WHERE precio BETWEEN value1 AND value2; 

SELECT precio 
from productos 
WHERE id BETWEEN 1 and 5;

SELECT max(precio)
FROM productos 
WHERE id BETWEEN 1 and 6;

```

</details>

<details>
  
  <summary> Ejercicios </summary>

1. Seleccionar todos los datos de aquellos
clientes que tienen el n??mero de DNI m??s alto.
2. Seleccionar la cantidad de clientes que est??n
registrados en la base de datos.
3. seleccionar el nombre y categor??a de aquellos
alojamientos que sirven para alojar a la mayor cantidad
de personas.
4. seleccionar el nombre y categor??a de aquellos
alojamientos que sirven para alojar a la menor cantidad
de personas.
5. ??Cu??l es la cantidad promedio de personas
que puede llegar a alojar la empresa?
6. ??De cu??ntos pisos es el alojamiento m??s
grande que ofrece la empresa?
7. ??Cu??l es el paquete de viaje m??s caro?
8. ??Cu??l es precio promedio de los paquetes de viaje?
9. ??Cu??l fu?? el ingreso total que producen las reservas
registradas?
10. ??Cu??ntas reservas se registraron para las fiestas
de fin de a??o? (desde el 23 de diciembre hasta 2 de Enero)
11. ??Cu??ntos alojamientos sirven para alojar hasta 3 personas?
12. ??Cu??ntas reservas realiz?? el cliente con id igual a 12?
13. ??Cu??l es la cantidad m??xima de personas que puede
alojar la empresa?

</details>


<details> 
  <summary> Enunciado 2 </summary>

-	Una empresa quiere sistematizar la gesti??n de su negocio, para ello decidi?? hacer un sistema donde pudiera controlar lo siguiente:
```
a.	Control de stock
b.	Clientes 
c.	Proveedores 
d.	Facturaci??n 	
```
 - Las tablas necesarias son:
```  
Clientes:
	cod_cliente
	dni o cuit
	nombre o raz??n social 
	direcci??n
	tel??fono 
	celular 
	fax
	mail
	website
	contacto
* los clientes pueden ser una empresa o una persona.

Productos:
	cod_producto
	descripci??n 
	stock
	precio unitario 
	stock m??nimo
	
*los productos tambi??n pueden ser servicios. Deber??n definir que atributos que pueden tener.

Proveedores:
	cod_proveedor
	cuit
	raz??n social 
	direcci??n
	tel??fono 
	fax
	mail
	website
	contacto

```
  
- Ejercicios

1.	Insertar 10 filas en cada tabla 
2.	Seleccione todos los datos de todas las filas de la tabla de clientes.
3.	Seleccione los datos del cliente nro. 6
4.	Seleccione apellido, nombre, tel??fono y celular de todos clientes cuyo apellido termine con ???ez???.
5.	Seleccione c??digo y descripci??n de todos los productos cuyo precio unitario sea mayor a $ 50.
6.	Borre los datos del cliente nro. 10
7.	Modifique la direcci??n del cliente nro. 10 a San Juan 1234
8.	Seleccione todos los productos cuyo stock m??nimo sea mayor a 3 
9.	Seleccione todos los productos con un precio unitario entre $20 y $100
10.	Seleccione todos los clientes que poseen website. 
11.	Borre todas las compras hechas al proveedor nro. 10 
12.	Modifique la direcci??n del proveedor nro. 3 a San Martin 12345
13.	Liste todas las compras realizadas el 01/04/2017
14.	Liste todas las compras del producto nro. 5 hechas al proveedor nro. 1 
15.	Liste los c??digos de producto que se compraron al proveedor nro. 5 por m??s de 10 unidades.

  
</details>

#### 3 de Junio

<details>
  
  <summary> Enunciado 1 </summary>
  
  
- Crear dos bases de datos:
  - personas
  - automotores

- Personas debe tener dos tablas:
  
- clientes:
  - Dni
  - nombre
  - Direcci??n
  - Tel??fono

- empleados:
  - Dni
  - Apellido y nombre
  - Direcci??n
  - Tel??fono
  - Mail
  - Cargo
  - edad

Automotores debe tener una tabla:

- Ambulancias:
  - Patente
  - nombreDeChofer


2) Proponer las consultas para realizar lo siguiente:
  
```
a. ingresar 5 filas de datos en cada tabla
b. agregar la columna "numeroDeSocio" en la tabla clientes
c. agregar la columna "numLegajo" en la tabla empleados
d. agregar la columna "numeroDeUnidad" en la tabla ambulancias
e. actualizar la direcci??n de dos clientes a elecci??n con el valor "Calle Falsa 123"
f. actualizar el mail de un empleado a elecci??n con el valor "hola@gmail.com"
g. actualizar el nombre del chofer de una ambulancia a elecci??n con el valor "Rodolfo"
h. eliminar a los empleados que tienen una edad mayor o igual a 65
i. eliminar a todos los clientes que tienen un n??mero de tel??fono menor al 40000000
j. eliminar a todos los clientes que se llamen "Equis"
```

</details>


<details>
  
  <summary> Enunciado 2 </summary>
  
  
- Una Empresa de Turismo quiere llevar una base de datos de sus Clientes, Paquetes de Viajes
(paquetes de viajes ya armados), Alojamientos, Reservas y Forma de Pago. 

```
Clientes:
id
Nombre
Apellido
Direcci??n
Dni
Tel??fono
Celular


Alojamientos:
id
Nombre
Categor??a
Direcci??n
Tel??fono
Cantidad de Personas
Cantidad de Pisos


Reservas:
(aqu??, el id de cliente y el id de alojamiento se ingresa a mano, no es autom??tico)
Cliente id
Alojamiento id
Paquete de viaje
Fecha de inicio
Fecha de fin
Cantidad de Personas
Lugar
Cantidad de d??as
Cantidad de noches
Precio
Cantidad de Excursiones
tipo de viaje (A??reo-Bus-Barco)
```

1.   Recordar que las consultas realizadas deben estar en un archivo .sql utilizando la herramienta Mysql Workbench.
2.   Elegir un nombre para la empresa de Turismo. Crear la base de datos utilizando el nombre elegido.
3.   Escribir los create de las tablas. 
4.   Insertar 20 filas en cada tabla. Las 20 inserciones deben ser realizadas mediante una sola consulta.
     Entre las inserciones correspondientes a la tabla de clientes, deben existir:
     - un cliente con el apellido "Garcia"
     - un cliente con el apellido "Garciorela"
     - un cliente con el apellido "Gimenez"
     - un cliente con el apellido "Juarez"
     - un cliente con el apellido "Haez"
5.   Seleccione todos los datos de todas las filas de la tabla de clientes.
6.   Seleccione los datos del cliente nro. 6 (utilizar la variable id..
7.   Seleccione apellido, nombre, tel??fono y celular de todos clientes cuyo apellido comience
con ???Gar???.
8.   Seleccione apellido, nombre, tel??fono y celular de todos clientes cuyo apellido termine
con ???ez???.
9.   Seleccione apellido, nombre, tel??fono y celular de todos clientes cuyo apellido contenga
     los caracteres ???ar??? en algun lugar del apellido.
10. Modifique la direcci??n del cliente nro. 10 a "San Juan 1234"
11. Borre los datos del cliente nro. 10
12.
a-  Seleccione todos los paquetes de viaje que tengan mas de 3 excursiones, los resultados deber??n estar ordenados
    alfab??ticamente por lugar.
b-  Seleccione todos los paquetes de viaje que tengan mas de 3 excursiones ordenados de mayor a menor por cantidad de d??as.
    
13. Seleccione todos los paquetes de viaje de dos d??as de duraci??n que cuesten mas de $6.000,50
14. Seleccione todas las reservas desde el 01/05/2017 hasta el 10/05/2017 ordenadas por
fecha descendente.
15. Borre todas las reservas pertenecientes al cliente nro. 10
16. Modifique la direcci??n del alojamiento nro. 3 a Belgrano 15897
17. Liste las reservas entre el 01/04/2017 hasta el 30/04/2017 para mas de 2 personas.
18. Borrar los datos del cliente nro. 6.
19. Agregar dos filas en la tabla Reservas donde los paquetes de viajes se llamen "Paquete Bariloche"
y sus dias y noches deber??n ser:
- 3 dias y 4 noches
- 10 dias y 11 noches
20. Modifique la cantidad de d??as y noches de los paquetes llamados "Paquete a Bariloche"; los nuevos d??as y noches ofrecidos deber??n ser de de 7 y 8, respectivamente.




  
</details>
