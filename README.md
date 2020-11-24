<div class="bg-primary">
  <p align="center">
  <a href="https://v5.getbootstrap.com/">
    <img src="https://idic.fi/wp-content/uploads/2020/08/Idic_Horizontal-Claro-150x50-1.png" alt="Idic logo" width="200">
  </a>
</p>
</div> 
<h3 align="center">REGLAS DE CODIFICACIÓN – “CLEAN CODE”</h3>
<p align="center">
  Favor leer antes de comenzar a codificar.
  <br>
  A continuación se mostrara las reglas de escritura que manejaremos en los diferentes lenguajes según sus estándares y sus recomendaciones.
  <br>
  <a href="https://idic.fi/"><strong>IDIC»</strong></a>
  <br>
  <br>
  <a href="https://estoesunaprueba.xyz/">Servidor de Pruebas</a>
  ·
  <a href="https://infoidic.com/">Servidor de Producci&oacute;n</a>
  ·
  <a href="#">Correo</a>
  ·
</p>

# Nota: Todo lo que se codea debe estar en ingles.

## Código Python - Django

### Guía: https://www.python.org/dev/peps/pep-0008/
### Sintaxis
- variables en minúscula: nombre y nombre_compuesto.
- Métodos: nombre y nombreCompuesto.
- Clases: Nombre y NombreCompuesto. 
- Aplicaciones: nombre
- Entornovirtual: idicprojectenv (nombre indiscutible).
- Dos saltos de línea entre clases y métodos
- Un salto de línea de los returns de los métodos.

### Recomendaciones
- Intentar que las líneas de código no superen 72 caracteres (por cuestión de Zen de python – legibilidad) en caso de ser así hay dos opciones: Salto de línea controlado con \ o Intentar manejar variables que reduzcan la línea en cuestión.
- Manejar el mismo archivo de .gitignore por seguridad ya que ha sido modificado especialmente para este proyecto.
- Algunas consultas especiales de este código no funcionan en SQLite; las que contienen distinct().
- El archivo de contraseñas se trabajan en un secret.json
- No hacer migraciones sin estar probadas previamente.


## Código JS
### Sintaxis
- variables en minúscula: nombre y nombre_compuesto.
- Métodos: nombre y nombreCompuesto.
- Clases: Nombre y NombreCompuesto. 
- Aplicaciones: nombre
- Entornovirtual: idicprojectenv (nombre indiscutible).
- Dos saltos de línea entre clases y métodos
- Un salto de línea de los returns de los métodos.

### Recomendaciones
- Por lo general JS torna a ser un código largo por cuestión de sus palabras reservadas de sistema y su sintaxis como tal, pero debemos intentar trabajarlo como python, claro esta sí es posible en caso de no pues trabajarlo como permita JS.
- Cuando se trabaja con urls Django con sintaxis como {%recoder:url_ejemplo%} estas solo funcionan en el mismos archivo html dentro de un <script>, debido a que el ciclo de vida se lee al mismo tiempo que el html y la data que nos genera el Django, de no ser así ese tipo de url no va a funcionar.


## Código SQL
### Sintaxis
- Tablas: Nombre y NombreCompuesto.
- Atributos: Nombre y Nombre_Compuesto. Nota de acá para adelante nombre y nombre_Compuesto.

### Recomendaciones
- En el models.py de Django tener en cuenta las reglas de sintaxis de SQL en los campos: db_columm y db_table.
- No usar entidades recursivas.


## Código CSS
### Sintaxis
- Variables en minúscula: nombre y nombre_compuesto.
- Clases: Nombre y NombreCompuesto.

### Recomendaciones
- Intentar que las líneas de código no superen 80 caracteres.
- Se codifica en SASS con llaves {}.


# General

### Nombre de Archivos 
nombre.py y nombre_archivo.py

### Recomendaciones
- Nunca hacer push a la rama master si no se tiene seguridad.
- Trabajar en las ramas que se les ha asignado.
- Comentar siempre cada método o clase con explicación de funcionamiento y de sus variables de entradas y su salidas.
- En el momento de importaciones de clases, métodos y constantes, favor solo importar lo necesario.
- En el momento de programar, primero hacer que funcione y después con el tiempo re-factorizar.
- En el momento de re-factorizar intentar hacer que se trabaje por clases con el fin de reducir código y poder heredarlo en otra funcionalidad.

### ¿Como Comentar Código?
- En ingles.
- Solo donde sea necesario y ser lo más claros posibles.
- La sintaxis depende del lenguaje; ejemplos de python:
Sí es un solo reglón:
```text
#Comentario
```
Sí es varios reglones usar:
```text
“”” 
 Comentario 
 Comentario 
“””
```
- En Clases o métodos:
```text
"""
	Reason: Convert a blank value to null, otherwise leave it 	the same.
	Method: None, Post, Get
	Input: string(pvar1, pvar2) or string(pvar1), dict(pvar2).
	Return: dictionary or string, etc.
"""
```


## Zen de Python:

- Bello es mejor que feo.
- Explícito es mejor que implícito.
- Simple es mejor que complejo.
- Complejo es mejor que complicado.
- Plano es mejor que anidado.
- Espaciado es mejor que denso.
- La legibilidad es importante.
- Los casos especiales no son lo suficientemente especiales como para romper las reglas.
- Sin embargo la practicidad le gana a la pureza.
- Los errores nunca deberían pasar silenciosamente.
- A menos que se silencien explícitamente.
- Frente a la ambigüedad, evitar la tentación de adivinar.
- Debería haber una, y preferiblemente solo una, manera obvia de hacerlo.
- A pesar de que esa manera no sea obvia a menos que seas Holandés.
- Ahora es mejor que nunca.
- A pesar de que nunca es muchas veces mejor que *ahora* mismo.
- Si la implementación es difícil de explicar, es una mala idea.
- Si la implementación es fácil de explicar, puede que sea una buena idea.
- Los espacios de nombres son una gran idea, ¡tengamos más de esos!
