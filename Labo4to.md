---

### Laboratorio de Algoritmos y Estructuras de Datos

----

#### [libro de consulta y ejercicios](https://github.com/nadianoe/nadianoe.github.io/blob/master/laboratorio4to/Nell%20Dale_%20Chip%20Weems%20-%20Programaci%C3%B3n%20y%20resoluci%C3%B3n%20de%20problemas%20con%20C++-McGraw%20Hill%20(2007).pdf)

----

#### 2 de Junio

<details>
	<summary> Ejercicio </summary>
	
- Crear un sistema que sirva para registrar datos de productos en venta y registrar las
ventas de dichos productos. 
- Por un lado, el sistema deberá proveer la funcionalidad de registrar productos y escribir
los datos (separados por comas) del mismo en un archivo con extensión csv.
- El archivo deberá tener el siguiente formato:
	``` nombre_de_producto,código,stock,costo,precio ```
	
- Cada registro de un nuevo producto deberá estar escrito en una nueva línea.
- El sistema también deberá:
	- permitir conocer el precio de un producto según el código.	
	- permitir conocer la ganancia que produce la venta de un producto según su código (ganancia = precio - costo)
	- permitir conocer los nombres de los productos disponibles según la letra inicial del nombre del producto
	- permitir conocer cuáles son los productos que tienen un stock igual a cero.
- Por otro lado, el sistema deberá recibir el nombre del producto, el código, el stock, el costo y el precio para
	luego agregar dichos datos en el archivo.
	


	
</details>

------

#### 31 de Mayo

- Trabajo práctico: 
	- Dos integrantes
	- Recordar que al programar, es recomendable distribuir las tareas que se realizan en funciones.
- [enunciado TP](https://github.com/nadianoe/nadianoe.github.io/blob/main/Trabajo%20Pr%C3%A1ctico%20N%C2%B01.pdf)

```c++
#include <stdlib.h>
#include <iostream>

using namespace std;

int generarValorAleatorio(int desde,int hasta){
    int numero;
    srand (time(NULL));
    numero = rand() % hasta + desde;
    return numero;
}

int main(){
     cout << generarValorAleatorio(1,10);

    return 0;
}
```

-----

#### 26 de Mayo

<details>
	<summary> Ejercicios </summary>
	
1. Crear uyna función que reciba como parámetro un nombre de archivo, una extensión y
luego retorne un string que contenga el contenido del archivo indicado.
	
</details>

-----

#### 24 de Mayo

<details> 
	<summary> Ejercicios </summary>

1. Crear una función que reciba como partámetros un char y un numero entero que representa una cantidad de líneas
   y deberá imprimir lo siguiente:
```
1. $
2. $$
3. $$$
...
```
2. Crear una funciòn que reciba un string y retorne un nuevo string compuesto por aquellos caracteres que
   tienen asociado un índice par.
3. Crear una funciòn que reciba un string y retorne un nuevo string compuesto por aquellos caracteres que
   tienen asociado un índice impar.
4. Crear una función que reciba un string y luego imprima cada tipo de letra que lo compone con su respectiva
   cantidad. Ejemplo: si se ingresa la palabra "ala", se imprimirá:
  ```
  cantidad de letra a: 2
  cantidad de letra l: 1
 ```	
	
</details>

------

#### 19 de Mayo

<details>
	<summary> Enunciado </summary>
	
1. Crear una función que reciba como parámetro un número y luego lo
   imprima 50 veces.
	
2. Crear una función que reciba como parámetro dos números y luego retorne
   el resultado de la siguiente operación:
```
	(( x^2 + x^3) / 3) + y^4 
```
3. Crear una función que reciba como parámetro un número mayor a cero y luego
   retornee la cantidad de múltiplos de 3 que existen desde el número -1000
   hasta el número ingresado.
4. Crear una función que reciba como parámetro un carácter (variable de tipo char) 
   y luego indique si el char recibido es vocal o no lo es. Para realizar esto,
   deberá retornar una variable de tipo bool.
5. Crear una función que reciba una palabra y luego retorne la cantidad de vocales que 
   contiene la palabra recibida.
	
</details>

-------

#### 17 de Mayo

<details>
	<summary> Enunciado </summary>
	
1. Realizar una función que muestre el siguiente menú y realice las siguientes operaciones:
```
1. Suma
2. Resta
3. Multiplicación
4. División
5. Salir
```
	
2. Realizar una función que reciba dos valores: horas y minutos y
muestre por pantalla cuánto tiempo falta para las 12:05 hs.
	
3. Realizar una función que reciba como argumento dos números. Uno de los números
   representará la base de una potencia; el otro, representará el exponente de una
   potencia. La función deberá retornar el valor de la potencia correspondiente.
   Utilizar un ciclo para las repetitivas multiplicaciones.

4. Realizar una función que reciba una cadena de texto y un
carácter. La función debe añadir al final de la cadena el carácter
enviado.
	
5. Realizar una función que reciba 3 números y luego retorne el número màs grande
   recibido.
   
6. Realizar un programa que reciba dos números correspondientes a la cantidad
   de filas y de columnas de una matriz, luego se deberá imprimir por consola
   una matriz de símbolos '@' teniendo en cuanta las dimensiones indicadas.
	
</details>

-----

#### 10 de Mayo

<details>
	<summary> Enunciado 2 </summary>

- Con respecto al enunciado anterior, realizar:
	
1. Crear un programa que escriba el resultado del punto 1 en un archivo llamado "tablasDel1Al10.txt".
2. Crear un programa que escriba en un archivo el resultado del ejercicio 3 para 5 nombres recibidos por consola.
   Todos los resultados deberàn estar en el mismo archivo.
3. Crear un programa que lea el archivo del punto anterior y luego imprimir la cantidad de letras "a" presentes
   en todo el archivo.
4. Crear un programa que sirva para registrar datos de personas. Se deberán pedir: nombre, apellido y edad.
Cada registro debrà estar escrito en un renglòn distinto y cada dato deberá estar separado por una coma.
El archivo deberá llamarse "datosDePersonas.csv".
</details>

<details> 
	<summary> Enunciado </summary>
	
------

### Laboratoria de algoritmos y estructuras de datos

#### Enunciado 10 de Mayo del año 2022

--------------

- Recuerde que los nombres de variables deben tener nombres
declarativos.

1. Crear un programa que imprima por consola las tablas
de multiplicación del 1 al 10 con el siguiente formato:
```
1 x 1 = 1
1 x 2 = 2
1 x 3 = 3
...

2 x 1 = 2
2 x 2 = 4
2 x 3 = 6
...

3 x 1 = 3
3 x 2 = 6
3 x 3 = 9
...

...

...

10 x 1 = 10
10 x 2 = 20
...
```

2. Crear un programa que reciba por consola un número positivo y luego
imprima por consola los números desde el 1 hasta el número recibido.

3. Crear un programa que reciba por consola un nombre y luego enumere
sus letras con el siguiente formato:
```
Nombre ingresado: Gloria.

Letras:

1° letra con índice 0 -> G
2° letra con índice 1 -> l
3° letra con índice 2 -> o
4° letra con índice 3 -> r
5° letra con índice 4 -> i
6° letra con índice 5 -> a
```

4. Crear un programa que reciba una palabra e imprima sólo
los caractéres con índices pares uno abajo del otro.

5. Teniendo en cuenta el siguiente programa,
``` c++
    string palabra;
    cin >> palabra;
    
    char primerLetra = palabra[0];
    char segundaLetra = palabra[1];
    
    string concatenacion = "";
    concatenacion = concatenacion + primerLetra;
    concatenacion = concatenacion + segundaLetra; 
```
modificarlo para que, mediante la concatenación, genere un
string que contenga la segunda mitad de las letras de la palabra
recibida y luego la imprima.

Por ejemplo, si se recibe la palabra "abecedario", deberá imprimir
el string "dario".

En caso de palabras con una cantidad de letras impar, deberá imprimir
las últimas 3 letras.

Además, la palabra recbida deberá tener más de 7 letras. En caso de
que no las contenga, deberá imprimir un mensaje pidiendo que 
ingrese una nueva palabra.

En caso de que el usuario ingrese "fin", el programa deberá finalizar.

</details>

------

#### 26 de Abril

<details>
	<summary> ejercicios </summary>
	
1. Crear un archivo y agregarle un contenido a elección.
Realizar un programa en el cual el usuario ingrese por consola el
nombre de un archivo a abrir, lo lea completamente e imprima su
información tal cual está escrita, por pantalla.
	
2. Pedir a un usuario 3 nombres y 3 números. Luego, escribir un
archivo con la cantidad de repeticiones correspondientes a cada número
recibido. Ejemplo: si se ingresó "Gloria" y el número 5, se deberá escribir
"Gloria" 5 veces.
	
3. Realizar un programa en el cual el usuario ingrese por consola el
nombre de un archivo a abrir y otro string con un nombre de
persona. El programa deberá indicar si el nombre recibido se encuentra escrito en el archivo.
	
4. Escribir en un archivo llamado "matriz.txt" la matriz generada en el ejercicio 8 
   correspondiente al día 18 de Abril.
	
</details>

<details>
	<summary> Ejemplo, manejo de archivos </summary>
	
```c++
#include <iostream>
#include <fstream>

using namespace std;

int main () {
    
    /*

	ifstream archivo;
	string frase;
	archivo.open("ejemplo.txt");
	archivo >> frase;
	archivo.close();
	cout << frase << endl;

	archivo.open("ejemplo.txt");
	getline(archivo, frase,'!');
	archivo.close();
	cout << frase << endl;

	ofstream archivo1;
	archivo1.open("ejemplo.txt",ios::app);
	cout << "Ingrese una frase" << endl;
	cin >> frase;
	archivo1 << frase << endl;
	archivo1.close();

	string frase;
	cout << "Ingrese una frase con espacios:" << endl;
	getline(cin,frase);
	cout << frase;
  
   */


    
    /**
    
    string frase;
	cout << "Ingrese una frase con espacios:" << endl;
	getline(cin,frase);
	cout << frase;
    **/
    /**
    int cantidadDeMayusculas = 0;
    int cantidadDeMinusculas = 0;
    
    for (int i = 0; i < str.size(); i++) {
        char letra = str[i];
        if ( isupper(letra) ){
            cantidadDeMayusculas++;
        } else {
            cantidadDeMinusculas++;
        }
        if (letra == ' '){
            cantidadDeEspacios++;
        }
    }
    
    cout << "Cantidad de mayúsculas: " << cantidadDeMayusculas << endl;
    cout << "Cantidad de minúsculas: " << cantidadDeMinusculas << endl;
    */
   
    
  return 0;
}
								      

	
```	
								      
</details>

<details>
	<summary> Ejemplo </summary>

```c++
	
int dia;
cin >> dia;
	
switch (dia) {
  case 1:
    cout << "Hoy is Sábado";
    break;
  case 2:
    cout << "Hoy is Domingo";
    break;
  default:
    cout << "Hoy es algún otro día de la semana";
}
```
	
</details>

----

#### 21 de Abril

<details>
	<summary> Ejercicios </summary>
	
- Realizar los ejercicios del 7 y 18 de Abril con ciclos "for".
	
</details>

<details>
	<summary> Propuesta de solución para ejercicio de matriz </summary>
	
```c++

#include <iostream>

using namespace std;

int main(){
    
    char caracter;
    string matriz;
    int cantidadDeCaracteresPorFila = 0;
    int cantidadDeFilas = 0;
    
    while(cantidadDeFilas < 10){
        
        cout << "Ingrese un caracter: " << endl;
        cin >> caracter;
        string fila;
        
        while (cantidadDeCaracteresPorFila < 10){
            fila = fila + caracter;
            cantidadDeCaracteresPorFila++;
        }
        
        cantidadDeCaracteresPorFila = 0;
        cantidadDeFilas++;
        
        fila = fila + "\n";
        matriz = matriz + fila;
        cout << "La fila generada es: " << fila << endl;
        fila = "";
        
    }
    
    cout << "La matriz es: \n" << matriz << endl; 
    
    return 0;
}

	
```
	
</details>

------

#### 18 de Abril

<details> 
	<summary> Ejercicios 1ra. parte </summary>
	
- Escribir programas con ciclos while para:
1. Imprimir en pantalla los números del 1 al 10.
2. Imprimir en pantalla los números del 10 al 1
3. Imprimir en pantalla los números de 2 al 20 incrementando de a dos (2, 4, 6, 8, etc.)
4. Imprimir en pantalla los números de 1 a 16 y sus valores al cuadrado al lado (1 – 1, 2 – 4, 3 – 9, 4 – 16, 5 – 25, etc.)
5. Que sume todos los valores del 1 al 10 y los imprima en pantalla.
6. Que imprima en pantalla todos los múltiplos de 6, desde 6 hasta 30 (6, 12, 18, 24 y 30).
7. Otra versión del ejercicio 5: que suma todos los valores del 1 al 100 y que, además de imprimir el resultado, 
   imprima el string  "1+2+3+4+5+.....".
8. Que imprima una matriz 10 x 10 que en vez de contener números, contenga repeticiones de un tipo de caracter por fila.
   El caracter deberá ser elegido por el usuario.

</details>


<details>
	<summary> Ejemplo - 2da. parte </summary>
	
```c++
#include <iostream>
#include <cctype>
using namespace std;

int main() {

  string nombre = "Gloria Flores";
  cout << nombre.size() << endl;
  cout << nombre.length() << endl;
  nombre.erase(4,1);
  nombre.erase(2);
  nombre.insert(1,"hola");
  nombre.substr(1,2);
  nombre.substr(3);
  cout << nombre << endl;

  char letra1 = tolower(nombre[3]);
  cout << letra1 << endl;
	
  char letra2 = toupper(nombre[3]);
  cout << letra2 << endl;

  return 0;
}

/**
https://www.cplusplus.com/reference/cctype/
https://www.cplusplus.com/reference/string/string/
*/
```
</details>
	
----

#### 12 de Abril

<details>

<summary> Ejercicio </summary>

1.
- Crear un programa que sirva para registrar los siguientes datos de productos:
    - nombre
    - precio
	
- El programa deberá proveerle al usuario las siguientes tareas:

* Registrar un producto.
  Aquí se deberá pedir el nombre del producto y su precio.

* Imprimir el importe parcial a pagar.
  - Aquí se deberá imprimir el importe a pagar por 
  los productos registrados hasta el momento.
  - Cuando se termine de mostrar el importe mencionado, 
  el programa deberá proveer la opción de realizar
  un nuevo registro.

* Finalizar registro. 
  Aquí se deberá imprimir el importe total a pagar.
  - Cuando se termine de mostrar el importe mencionado, 
  el programa no deberá dar la opción de realizar 
  un nuevo registro.
  
2. Realizar un programa donde se ingresen dos números
(primero el menor, luego el mayor) y luego se muestren todos los
números intermedios (incluyendo los extremos).
	
</details>

<details>
	<summary> Ejemplo1 </summary>

```c++

#include <iostream>

using namespace std;

int main (){

  string palabra = "casa";
  // c - 0, a - 1, s - 2, a - 3
  cout << palabra[3] << endl;  
  
  string str1, str2, str3, str4;
  
  str1 = "Esto es un a frase#$#$&$56";  
  
  char caracter1 = 'f';
  char caracter2 = '#';
  
  bool comparacion = caracter1 == caracter2;
  
  //str2 = 'x'; // "x"
  str2 = "hojaldre";

  cin >> str2;
  int size = str2.size();

  str2 = "empa\"nada"; // empa"nada
  cout << str2 << endl;
  
  str2 = str2 + " hola"; // hoja hola
  
  cout << str2 << endl;
  str4 = "hola";
  
  str2 = "def";
  str1 = "abc";
  str3 = str1 + str2;
  
  string nombre = "Gabriela";
  int indice = 1;
  cout << nombre[indice + 2] <<  endl;
  
  nombre[0] = 'a'; //aabriela
  nombre[2] = 'j'; //aajriela
  nombre[5] = ' '; //aajri la
  
  cout << nombre <<  endl;

  cout << str3  << '\n';
  
  return 0;
}
		   
```
	
</details>
	
<details>
	<summary> Ejemplo 2 </summary>
	
```c++
#include <iostream>
#include<string>

using namespace std;

int main() {

    string nombre;
    cin >> nombre;
    
    char letra1 = nombre[0];
    char letra2 = nombre[1];
    
    cout << letra1 << endl;
    cout << letra2 << endl;
    
    string concatenacion = "";
    concatenacion = concatenacion + letra1;
    concatenacion = concatenacion + letra2;
    
    cout << "valor nuevo: " << concatenacion << endl;
    

  return 0;
}
	
```	
</details>

<details>

<summary> Ejercicios con strings </summary>

1. Realizar un programa donde el usuario ingrese una palabra y se
muestren todas las letras de la palabra separadas por un salto de
línea (una letra por renglón).
2. Realizar un programa donde el usuario ingrese dos cadenas de
texto y el programa compare la última letra de ambas cadenas y
muestre si son o no iguales.
3. Realizar un programa en donde el usuario ingrese una cadena de
texto y luego una letra. Se deberá mostrar la cadena con su última
letra cambiada por la ingresada.
4. Realizar un programa que reciba una cadena de texto y devuelva
el número de minúsculas y mayúsculas.
5. Realizar un programa que muestre el reverso de una cadena de
texto. Por ejemplo: el reverso de “asado” es “odasa”.
	
</details>

----
#### 7 de Abril

<details>
	<summary> Ejercicios </summary>

1. Realizar un programa que imprima por pantalla los números del 1 al 2000.
	
2. Realizar un programa que le permita realizar *repetitivamente* el ingreso
de un número y luego imprimir el resultado de multiplicar ese número por dos.
La repetición deberá suceder hasta que el usuario ingrese el número cero.
	
3. Realizar un programa que le permita al usuario ingresar 5 números y luego 
imprimir el resultado correspondiente a la suma de los números ingresados.

4. Realizar los ejercicios 1 y 2 de la página 246.
	
</details>

----
	
#### 5 de Abril

<details>
	<summary> Ejercicio integrador </summary>
Crear un programa que reciba un número y luego indique si el número ingresado pertenece
al conjunto A, al conjunto B, al conjunto C o a todos los conjuntos.
	
```
 A = (1, 10) U (130, 1000] 
 B = [-1, 3)  U (500, 800)
 C = (0, 5000) U [5001, +infinito)
```
	
Tener en cuenta que:
	
```
A ∩ B ∩ C = (1,3] U (500, 800)
```
	
</details>


<details>
	<summary> Exámen </summary>
	
1. Calcular y comentar los valores de verdad de las variable a, b y f en aquellas líneas donde aparecen.
Copiar todo el código en un archivo llamado ejercicio1_29deMarzo.cpp y colocar las respuestas como comentarios de  c++.

```c++
int main(){
	
	bool a = true;
	bool b = false;
	int c = 0;
	int d = 123;
	int e = 100;
	bool f = c == 0;
	f = c > 12;
	f = d > 89;
	f = e >= 100;
	f = e > 100;
	f = (f && e == 5) || c == 0;
	f = !a || d == 0;
	f = d == 0;
	f = d != 0;
	f = !b && e != 0;
	c++;
	f = c == 90;
	c++;
	d--;
	f = c > 90 && d < 0;
	f = !b || !f;
	a = !f && d > 0;
	e++;
	b = e == 12 || e == 13;
	a = (false && !false) || (!true || false)
	a = (d > 0 && d <= 100) || (c != 9)
	f = !(true || false) || (a == false)

}
```

2. Crear un algoritmo mediante diagramas de flujo que sirva para indicar si un número ingresado por el usuario es par o impar.
3. Sea 
```		      
 A = [-3,4] U (12,900) y B = (550,4000)  U (5000,+inf)
```
Crear un algoritmo mediante diagramas de flujo que reciba un número y luego indique si el mismo pertenece
a A, B o a ambos conjuntos.
4. Crear un algoritmo mediante diagramas de flujo que reciba un nombre, un apellido y una edad y luego imprima un saludo que cumpla con el siguiente formato: 
```
Los datos ingresados son los siguientes:
- Nombre: Gloria
- Apellido: Flora
- Edad: 88
```
En el ejemplo, los valores ingresados fueron: Gloria, Flora y 88

5. Implementar los algoritmos creados en los puntos 2, 3 y 4 utilizando el lenguaje de programación c++.
Cada ejercicio deberá estar en un mismo archivo. 
- Se deberá proveer un menú de opciones: 
	- opción 1, utilizar aplicacion de ejercicio 2
	- opción 2, utilizar aplicación de ejercicio 3
	- opción 3, utilizar aplicación de ejercicio 4
- Cuando el usuario elija e ingrese una opción, se deberá poder utilizar la aplicación elegida y luego deberá finalizar el programa.
			      
</details>
	
----
#### 31 de Marzo

<details>
<summary> Ejercicios  </summary>  
- Página 202, ejercicio 3 y ejercicio 6
</details>

----

#### 29 de Marzo

<details>
<summary> Exámen  </summary>  


1. Calcular y comentar los valores de verdad de las variable a, b y f en aquellas líneas donde aparecen.
Copiar todo el código en un archivo llamado ejercicio1_29deMarzo.cpp y colocar las respuestas como comentarios de  c++.

```c++
int main(){
	
	bool a = true;
	bool b = false;
	int c = 89;
	int d = 0;
	int e = 12;
	bool f = c == 0;
	f = c > 12;
	f = c > 89;
	f = c >= 89;
	f = f && e == 5;
	f = !a || d != 0;
	f = d == 0;
	f = d != 0;
	f = !b && e > 0;
	c++;
	f = c == 90;
	c++;
	d--;
	f = c > 90 && d < 0;
	f = b && !f;
	a = !f && d > 0;
	e++;
	b = e == 12 || e == 13;
	a = (true && !false) || (false || false)
	a = (d > 0 && d < 100) || (c == 89)
	f = !(true || false)

}
```

2. Crear un algoritmo mediante diagramas de flujo que sirva para indicar si un número ingresado por el usuario es impar y menor a 100, en caso de que el número ingresado no cumpla con los requisitos, deberá imprimir "No es impar y menor a 100".
3. Crear un algoritmo mediante diagramas de flujo que reciba un número y luego indique si el mismo es positivo, negativo o igual a cero.
4. Crear un algoritmo mediante diagramas de flujo que reciba dos nombres y luego imprima un saludo que cumpla con el siguiente formato: "¡Hola, Gloria y Walter!" (en este caso, los nombres ingresados fueron Gloria y Walter).
5. Implementar los algoritmos creados en los puntos 2, 3 y 4 utilizando el lenguaje de programación c++.
Cada ejercicio deberá estar en un mismo archivo. 
- Se deberá proveer un menú de opciones: 
	- opción 1, utilizar aplicacion de ejercicio 2
	- opción 2, utilizar aplicación de ejercicio 3
	- opción 3, utilizar aplicación de ejercicio 4
- Cuando el usuario elija e ingrese una opción, se deberá poder utilizar la aplicación elegida y luego deberá finalizar el programa.

			      
</details>

----
#### 22 de Marzo

<details>
<summary> Ejercicios </summary>  

1. Capítulo 5
- Ejercicios de preparación para exámen
	- Página 198, ejercicios 5 y 10
	- Página 199, ejercicios 14 y 15

- Ejercicios de calentamiento para programación
	- Página 199, ejercicio 1
	- Página 200, ejercicio 10	
2. Crear una aplicación que sirva para calcular el área de un triángulo siendo la base y la altura ingresadas por el usuario (recordatorio: area = (base * altura) / 2 para cualquier tipo de triángulo).
3. Crear una aplicación que sirva para realizar las cuatro operaciones básicas (suma, resta, división y multiplicación) con dos números ingresados por el usuario. El usuario deberá elegir qué operación realizar.
4. Modificar el programa del ejercicio anterior para que se muestre un mensaje de error si se intenta dividir por cero (recordatorio: 0/k = 0, k/0 = indefinido para cualquier k).
5. Realizar una aplicación que calcule el monto total a pagar por cada cliente de una librería. El sistema deberá recibir la cantidad de libros que comprará el cliente y luego imprimir el monto total a abonar. 
Con respecto a los precios de los libros, todos los libros cuestan $300 pero llevando más de 5 libros cuestan $250 c/u.
6. Realizar un programa donde el usuario ingrese un número y que muestre por pantalla si el mismo es par o impar

</details>

---

#### 17 de Marzo
<details>
<summary> Ejemplo de exámen </summary>  

1. Calcular y comentar el valor de verdad de las siguientes expresiones.

```c++
int main(){
	
	int a = 5;
	int b = 6;
	bool c = true;
	bool d = a <= 5;
	d = a >= 100;
	d = a == 6;
	d = !(a == 6);
	d = a == b;
	b--; 
	d = a == b;
	a++;
	d = b == a;
	b = 2;
	a = 1;
	d = a > -10 && a < 10;
	d = b <= 2 || b >= 200;
	d = b == 1 || b == 22;
	d = a < 5 && b > 0;
	d = a >= 70 && true;
	d = false || b <= 10;
	d = a == 1 || a == -1;
	d = a > 1 || a < -1;
	d = (true && false) || (true && true);
	d = (false || true) || (true && false);
	d = !d;
	d = d && d;
	d = d || d;
	d = (!d) || d;

}
```

2. Crear un algoritmo mediante diagramas de flujo que sirva para recibir un número y
luego indicar si el mismo es mayor o igual a 19. En caso de que no lo sea, deberá imprimir
"intente nuevamente".
3. Crear un algoritmo mediante diagramas de flujo que sirva para recibir un nombre y 
luego imprimir una triplicación del mismo.
Es decir, por ejemplo, si el ususario ingresa "Gloria", el algoritmo deberá imprimir
"GloriaGloriaGloria".
4. Crear un algoritmo mediante diagramas de flujo que reciba dos números e indique si uno de ellos es la triplicación del 
otro. Es decir, por ejemplo, si el ususario ingresa el 3 y el 9, el algoritmo deberá imprimir
"El segundo número es la triplicación del primero"´; en caso contrario, deberá imprimir "El primer número
es triplicación del segundo" o "intente nuevamente". (Incluir la utilización de un "else if").
5. Implementar los algoritmos creados en los puntos 2, 3 y 4 utilizando el lenguaje de programación c++.
Cada ejercicio deberá estar en un mismo archivo. 
- Se deberá proveer un menú de opciones: 
	- opción 1, utilizar aplicacion de ejercicio 2
	- opción 2, utilizar aplicación de ejercicio 3
	- opción 3, utilizar aplicación de ejercicio 4
- Cuando el usuario elija e ingrese una opción, se deberá poder utilizar la aplicación elegida y luego
  deberá finalizar el programa.


</details>

---

#### 15 de Marzo

<details>

<summary> Ejemplo  </summary>  

```c++
#include <iostream>

using namespace std;

int main(){
    
    /* Sea A un conjunto tal que 
       
       A = (-∞,2) U [4,10]
      
    */
    
    int a = 5;
    
    
    if(a < 2){
        cout << "Es menor a 2. Pertenece a A."  << endl;
    } else if (a >= 4 && a <= 10){
        cout << "Está entre 4 y 10. Pertenece a A" << endl;
    } else {
        cout << "No pertenece a A."<< endl;
    }
    
    a = a + 1;
    a = a - 1;
    a = 2 * a;
    a = a + 2;
    a = a + 1;
    a++;
    a = a - 1;
    a--;
    
    int b,c,d;
    
    b = 1;
    b++;
    c = b;
    
    cout << c << endl;
    
    /** negación **/
    
    bool f = true;
    f = !f; // false
    f = b > 90;
    f = !(b > 2);
    
    /** trabajo con strings **/
    
    string d = "hola";
    d = d + d; // "holahola"
    string e = "chau";
    e = e + d; // "holaholachau"

    return 0;
}
```
</details>

<details>

<summary> Enunciado </summary>

1. Crear una variable de tipo int que se llame "num1" y contenga al número 10
2. Crear una variable de tipo string que se llame "palabra" y contenga el dato "abcdef"
3. Crear una variable de tipo bool que se llame "esCierto" y contenga el dato false
4. Cambiar el valor de la variable "num1", la misma deberá contener el valor que contiene
pero incrementado en 1.
5. Cambiar el valor de la variable "palabra", la misma deberá contener 3 repeticiones del
valor que ya contiene.
6. Cambiar el valor de la variable "esCierto", la misma deberá contener la negación del valor 
que ya contiene.
7. Cambiar el valor de la variable "num1", la misma deberá contener el doble del valor que
ya contiene.
8. Crear una variable de tipo int que se llame "num2" y contenga el valor de la variable "num1"
incrementado en 4
9. Modificar el valor de la variable "num2", la misma deberá contener el valor que contiene pero disminuido en 2

</details>

----

#### 10 de Marzo

<details> 

<summary> Material extra visto en clase </summary>

- [diapositivas](https://github.com/nadianoe/nadianoe.github.io/blob/master/laboratorio4to/Clase%203_C++.pdf)
- [tablas de verdad](https://raw.githubusercontent.com/nadianoe/nadianoe.github.io/master/laboratorio4to/tabladeverdad.jpg)

</details>


<details> 

<summary> Ejemplo </summary>

```c++
#include<iostream>

using namespace std;

int main(){

	// este es un comentario de una línea

	/* 
	este es un 
	comentario
	de varias lineas
	*/

	/**
	enteros -> int
	cadenas "sdgdfg" "3453#$%#$&/"  -> string
	decimales -> float
	bool -> true , false
	**/


	/* imprimir por consola */
	cout << "aaaaaa" << endl;

	cout << "bbbbbb" << endl;

	cout << "cccccc" << endl;

	/** pedir un número por consola **/
	cout << "Ingrese un número" << endl;

	int numero = 234;
	numero = 23;
	numero = 45;

	string hola = "Nadia     &/$%&)()"; 
	
	int numero1;
	cin >> numero1;
	cout << "El número ingresado fue: " << numero1 << endl;

    	/** pedir un nombre por consola **/
	cout << "Ingrese un nombre" << endl;
	string nombre;
	cin >> nombre;
	cout << "El nombre ingresado fue:" << nombre << endl;


	/**
	int f = 4;
	int g = 1;
	int suma = f + g; // 5
	string h = "1";
	string i = "5";
	string c = h + i; // "15"
	**/



	/**
	    comparadores: 
		== , != , < , >, <= , >= 
   	**/

	int a = 23;
	int b = 1;

	bool condicion = a == 34;
	condicion = a != 4;
	condicion = a > 3;
	condicion = a >= 5;
	condicion = a <= 100;
	condicion = a == b;
	condicion = a < b;
	condicion = a == 23;
	condicion = false;
	condicion = true;
	condicion = false && false;
	condicion = false || true;
	condicion = !true;
	condicion = b > 0 && b < 10;


	if (condicion){
		cout << "hola"<< endl;
	} else {
		cout << "chau" << endl;
	}

	cout << "fin";

	return 0;
}
```
</details>


<details> 

<summary> Enunciado </summary>

- Programar en c++ los algorimos realizados la clase pasada.
- Cada ejercicio debe estar en un archivo separado.

</details>

----

#### 8 de Marzo 


<details>

<summary> Diapositivas </summary>

- [diapositivas, parte 1](https://github.com/nadianoe/nadianoe.github.io/blob/master/laboratorio4to/Clase%201_%20Introducción%20al%20Laboratorio.pdf)
- [diapositivas, parte 2](https://github.com/nadianoe/nadianoe.github.io/blob/master/laboratorio4to/Clase%202_%20Sentencias%20condicionales.pdf)

</details>

<details>
<summary> Ejercicios </summary>

1. Crear un algoritmo que reciba dos números y luego indique cuál es el número mayor.
2. Crear un algoritmo que reciba un número y luego indique si el nùmero recibido es igual o distinto a 800.
3. Crear un algoritmo que reciba un número e indique si el nùmero recibido es mayor a 100 o  menor a 50.
4. Crear un algoritmo que reciba un número e indique si el nùmero recibido es mayor a 18 y menor a 90.
5. Crear un algoritmo que reciba la edad del usuario y luego indique si es mayor o menor de edad.
6. Crear una aplicación que le muestre un menú al usuario. El menú deberá ofrecerle realizar 2 operaciones:
   - sumar 3 números
   - calcular el promedio de 3 números
   
La aplicación deberá retornar el resultado calculado.

</details>

----

