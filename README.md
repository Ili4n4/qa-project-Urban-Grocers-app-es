# Proyecto Urban Grocers 

Descripción:

El objetivo del proyecto es crear un kit 
de productos para el usuario,ejecutando
las pruebas positivas y negativas en base
a los requisitos de la solicitud.
También se revisarán los códigos de 
respuesta esperados y actuales.

Pasos a seguir:
1. Conectar GitHub con Tripleten
2. Clonar el repositorio en la computadora
3. Trabajar con el proyecto de forma local
4. Crear un kit para el usuario
5. Entrega de proyecto


Tecnologías:
PyCharm
GitHub

Documentación Urban Grocers
+Creación de cuenta
+Creación de kits

Instalaciones
+pip
+requests
+pytest

Lista de comprobacion:

Lista de comprobación de pruebas

1	El número permitido de caracteres (1): 
kit_body = { "name": "a"}	
Código de respuesta: 201 
El campo "name" del cuerpo de la respuesta coincide con el campo "name" del cuerpo de la 
solicitud

2	El número permitido de caracteres (511):
kit_body = { "name":"El valor de prueba para esta comprobación será inferior a"}
Código de respuesta: 201 
El campo "name" en el cuerpo de la respuesta coincide con el campo "name" en el cuerpo 
de la solicitud

3	El número de caracteres es menor que la cantidad permitida (0):
kit_body = { "name": "" }	
Código de respuesta: 400

4	El número de caracteres es mayor que la cantidad permitida (512):
kit_body = { "name":"El valor de prueba para esta comprobación será inferior a” }	
Código de respuesta: 400

5	Se permiten caracteres especiales:
kit_body = { "name": ""№%@"," }	
Código de respuesta: 201 
El campo "name" del cuerpo de la respuesta coincide con el campo "name" del cuerpo 
de la solicitud

6	Se permiten espacios:
kit_body = { "name": " A Aaa " }	
Código de respuesta: 201 
El campo "name" del cuerpo de la respuesta coincide con el campo "name" del cuerpo de la
solicitud

7	Se permiten números:
kit_body = { "name": "123" }	
Código de respuesta: 201 
El campo "name" del cuerpo de la respuesta coincide con el campo "name" del cuerpo de 
la solicitud

8	El parámetro no se pasa en la solicitud: 
kit_body = { }	
Código de respuesta: 400

9	Se ha pasado un tipo de parámetro diferente (número):
kit_body = { "name": 123 }	
Código de respuesta: 400