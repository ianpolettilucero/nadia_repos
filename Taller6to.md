
----
###  Taller de Tecnologías de Soporte Informático - 6to
----


#### 9 de Junio

<details>
	<summary> Ejemplo </summary>
	
```python
import pandas as pd
import matplotlib.pyplot as plt1
import numpy as np

valor = np.nan #NaN
	
df1 = pd.read_csv("../data/vacunasCovid19.csv")
df1 = df1.dropna()
	
x_values = df1['grupo_etario'].unique()
y_values = df1['grupo_etario'].value_counts().tolist()
y_values.reverse()
plt1.figure(figsize=(8,6))
plt1.barh(x_posiciones, y_values)
plt1.xticks(x_posiciones, x_values)
plt1.xticks(rotation=90,fontsize=10)
	
#####################################################################
	
def convertir_en_minusculas(valor):
  if type(valor) == str:
    return valor.lower()
  else:
    return valor

# ejemplo 2
def arreglar_fecha(valor): 
  valor = str(valor)
  for caracter in valor:
    if not caracter.isnumeric() and caracter != "/"
      valor = valor.replace(caracter,'/')
  return valor

df2 = df1.applymap(convertir_en_minusculas)
	
df3['nombre_de_columna'] = df1['nombre_de_columna'].apply(convertir_en_minusculas)

df4['Precio'] = df1['Precio'].apply(float)


columna_precio = df4['Precio']

for indice, valor in columna_precio.items():
    print("indice: ",indice)
    print("valor: ",valor)
	
```
</details>

<details>
	<summary> Enunciado </summary>	


- Limpiar el siguiente set de datos:
```
Edad, Altura, Peso, Promedio, Sexo, LU, Observación 
25, 1.80, 83, 7.79, H, 125/89, ninguna
21, 1.89m, 86, 9.7, H, 35 88, ninguna
39, 1.54, 50, 7.1, M, 142-80, hipertension
49, 1.66, 70, 6.54, Mujer, 553/83, ninguna
31, 1.70, 81, 7.21, H, 495-83, hiper tension
33, 1.74, 93 kg, 7.1, Hom, 25/78, sobrepeso
29, 1.81, 82.5, 6.9, H, 445//81, ninguna
19, 1.82, 86.3, 8.43, H, 5/84, NINGUNA
20, 1.76, 75, 10, M, 1/81, gripe
65,, 70, 4.21, M, 1455-89, no hay
32, 1.64, 60, 9.10, M, 400-80, ninguna
59, 1.70, 67, 8.99, men, 100/89, ninguna
34, 1.81, 97, 7.46, H, 1/89,  
49, 1.78, 432, 7.41, Hombre, 500\86, dolor cabeza
51, 1.77, 75, 9.10, H, 25/85, hipertenso
52, 1.65, 64, nan, M, 22\84, ninguna
40, 1.69, 70, 6.00,m, 35/89, ninguna
41, 1.80, 8, 9.2, H, 099/89, no hay obs
25, nan, 72, 6.29, M, 90.80, nada
28, 1.68, 68, 7.54, M, 145/81, ninguna
29, 1.81, 83, nan, H, 111/83, NINGUNA
```
- El resultado final deberá ser igual a la siguiente versión:
```
Edad,Altura,Peso,Promedio,Sexo,LU,Observación 
0,25,1.80,83,7.79,h,125/89,ninguna
1,21,1.89,86,9.7,h,35/88,ninguna
2,39,1.54,50,7.1,m,142/80,hipertension
3,49,1.66,70,6.54,m,553/83,ninguna
4,31,1.70,81,7.21,h,495/83,hipertension
5,33,1.74,93,7.1,h,25/78,ninguna
6,29,1.81,82.5,6.9,h,445/81,ninguna
7,19,1.82,86.3,8.43,h,5/84,ninguna
8,20,1.76,75,10.0,m,1/81,ninguna
10,32,1.64,60,9.1,m,400/80,ninguna
11,59,1.70,67,8.99,m,100/89,ninguna
12,34,1.81,97,7.46,h,1/89,ninguna
13,49,1.78,432,7.41,h,500/86,dolor de cabeza
14,51,1.77,75,9.1,h,25/85,hipertension
17,41,1.80,8,9.2,h,099/89,ninguna
19,28,1.68,68,7.54,m,145/81,ninguna	
```
- El archivo .ipynb a entregar deberá contener todas las funciones que fueron necesarias realizar para lograr que 
el set de datos tenga un resultado final como el propuesto.
	
</details>
	
------

#### 19 de Mayo

<details> 
	<summary> Ejercicio </summary>

- Buscar y descargar un nuevo dataset .csv que tenga, al menos, 500 líneas.
- Formular al menos 5 preguntas que podrían ser respondidas con la información 
del data-set elegido.
- Responder las preguntas formuladas.

- Comentario: deberán crear los gráficos que considere necesarios para responder
las preguntas propuestas. 
El propósito es generar una serie de argumentos basados en la información que provee el data-set.
- Crear un breve informe donde se enumeren las preguntas propuestas y
las respuestas obtenidas.
	
</details>

------
	
#### 5 de Mayo

<details>
	<summary> Ejemplo y enunciado </summary>

- Ejemplo:
	- [link hacia el archivo grafico1.ipynb](https://github.com/nadianoe/nadianoe.github.io/blob/main/graficos1.ipynb)
	
- Enunciado:
	
1. Realizar dos de gráficos utilizando .bar() y utilizando .plot() 
para 2 columnas a elección presentes en sus archivos csv.

2. Debajo de cada gráfico deberán realizar escribir un análisis
donde se respondan las siguientes preguntas:

- ¿Qué conclusión o conclusiones sacaría del gráfico obtenido?
- ¿Cuáles serían las variables que considera que deberían tenerse en
cuenta pero no las puede apreciar porque el csv no se las provee?
¿Porqué?
- ¿Podría relacionar los datos de las dos columnas elegidas para especular
y proponer una conclusión?
En caso de que no, ¿Con qué columnas cree que lo podría hacer? ¿Porqué?

- El trabajo realizado deberá estar escrito en un archivo .ipynb, mezclando
  gráficos, código python y texto.
	
</details>

-----

#### 21 de Abril

<details>
	<summary> Ejemplo </summary>
	
```python
	
import pandas as pd
df = pd.read_csv("datos_nomivac_covid19.csv")
df = pd.read_csv("datos_nomivac_covid19.csv",sep=";",engine="python")
print(df)
print(list(df.columns))
print(list(df.index))
print(df['grupo_etario'])
df.loc[0:1000]
df.loc[[1,5,8]]
dfConIndiceDNI = df.set_index('DNI')
df['sexo'].value_counts()
df_2 = df.drop_duplicates()
df.to_csv("nuevo.csv")
	
```
- [notebook](https://github.com/nadianoe/nadianoe.github.io/blob/master/taller6to/exp.ipynb)
	
</details>

<details> 
	<summary> Enunciado </summary>
	
1) Leer su archivo csv utilizado.
	
2) De ser posible, elegir una columna que pueda servir como índice y setearla como tal.
	
3) Eliminar las filas duplicadas
	
4 Escribir un nuevo archivo .csv con las modificaciones realizadas
	
5) Colocar en forma de tabla, las primeras 3000 filas  y luego, las ultimas 2000.
Si su archivo csv no tiene una cantidad de datos que cumpla lo pedido, 
la tabla deberá tener las primeras 300 y las últimas 200.

6) Imprimir el data frame escrito en el nuevo archivo .csv
	
7) Colocar en forma de tabla las filas 1, 5, 12, 36.
	
8) Imprimir una lista con los nombres de todas las columnas.
	
9) Imprimir los datos de una columna a elección.
	
</details>

----

####  31 de Marzo

<details> 
	<summary> Enunciado </summary>
	
- Elegir una API y realizar las peticiones necesarias para crear un set de datos
- Utilizar el separador ","
- El set de datos obtenido deberá tener
  - extensión .csv
  - al menos 30 lineas 
  - al menos 3 columnas.


</details>

<details> 
	<summary> Ejemplo </summary>

```python
import requests


if __name__ == '__main__':

    archivo = open("hola.csv", "w")
    nombres_columnas = "mensaje , status \n"
    archivo.write(nombres_columnas)
    archivo.close()
    
    for i in range(10):
        respuesta = requests.get('https://dog.ceo/api/breeds/image/random')
        respuesta.status_code
        informacion = respuesta.json()
        mensaje = informacion["message"]
        estado = informacion["status"]

        linea = mensaje + "," + estado + "\n"

        archivo = open("hola.csv", "a")
        archivo.write(linea)
        archivo.close()
```
</details>

-----

#### 10 de Marzo

<details>
<summary> Ejemplo  </summary>

```python
print("hola")
print("Hola", "Holaaaa")
cadenas = "Holaaa" + "Hola" + 'Holaaaaaaa'
print(cadenas)

num1 = 34
num2 = 2
suma = num1 + num2
print(suma)

num1 = 23.0
num2 = 0.5
print(num1 + num2)

lista = [1, 2, 3, 5, 6, 4, 4, 4, 4]
lista.sort()

lista = ["afdf", 22, "hola", 2, 6.78]
print(lista)

if (len(lista) == 2):
	print("tiene dos elementos")
else:
	print("tiene más de dos elementos")

a = 1
b = 3
if b > a:
	print("b es mayor")
elif a == b:
	print("a y b son iguales")

for i in range(5):
	print(i)

for elemento in lista:
	print(elemento)

while b > a:
	print("abcd")
	a = a + 1

diccionario1 = {"Ana": 12, "Fabio": 3}
diccionario1["Lolo"] = 33
diccionario1['Lola'] = 90
valores = diccionario1.values()
valores = list(valores)

for clave in diccionario1.keys():
	valor = diccionario1[clave]
	print(clave,valor)


print(diccionario1)
print(valores[0])

set = {"Jazmín", "Karina"}
set.add("Paola")

print(set)

for elemento in set:
	print(elemento)


numero_ingresado = input()
numero = int(numero_ingresado)

nombre_ingresado = input("Ingrese un nombre")
print(nombre_ingresado)



'''
documentación sobre listas:
https://python-reference.readthedocs.io/en/latest/docs/list/
documentación sobre conjuntos:
https://python-reference.readthedocs.io/en/latest/docs/sets/
documentación sobre diccionarios:
https://python-reference.readthedocs.io/en/latest/docs/dict/
'''
```

</details>

<details>
<summary> Enunciado </summary>

1. Crear una lista que contenga 1000 números enteros. Los mismo deberán ser agregados
mediante un ciclo for y utilizando la función range.
2. Tomar la lista creada en el punto anterior y eliminar los elementos con índices pares.
3. Crear un set que contenga 3 nombres ingresados por consola.
4. Tomar el set creado y eliminar los nombres que comiencen con la letra a.
5. Crear un diccionario que contenga 2 o más nombres de sus compañeros con sus respectivas
edades.
6. Tomar el diccionario creado y multiplicar las edades por 2, mediante un ciclo for.
7. Crear el famoso juego de la vivorita utilizando las estructuras de datos vistas.
El mismo deberá utilizarse y visualizarse por consola.
</details>

----
