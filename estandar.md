# Cómo funciona el formato Markdown

Este archivo contiene todo el estándar soportado por el formato **Markdown**.

<small>Actualización: **12/12/2020**.</small>

---

Encabezados
===========

```markdown
# Título 1
## Título 2
### Título 3
#### Título 4
##### Título 5
###### Título 6

Alternativamente para los títulos 1 y 2:

Título 1
========

Título 2
---
```

# Título 1
## Título 2
### Título 3
#### Título 4
##### Título 5
###### Título 6

Alternativamente para los títulos 1 y 2:

Título 1
========

Título 2
---

Enfásis
=======

```markdown
Escritura itálica with *asteríscos* o _guión bajo_.

Negrita o enfatizada con **doble asteríscos** o __doble guión bajo__.

Un ejemplo para cobinar ambos **asteríscos y _guión bajo_**.

Para texto tachado usar dos virgulillas (tildes): ~~tachar esto~~.
```

Escritura itálica with *asteríscos* o _guión bajo_.

Negrita o enfatizada con **doble asteríscos** o __doble guión bajo__.

Un ejemplo para cobinar ambos **asteríscos y _guión bajo_**.

Para texto tachado usar dos virgulillas (tildes): ~~tachar esto~~.

Listas
======

(En este ejemplo los espacios iniciales son representados con puntos: .)

```markdown
1. Primer elemento de una lista numerada.
2. Otro elemento.
..* Un elemento de una lista con viñetas.
1. El nro. utilizado no tiene importancia, será calculado de forma automática.
...1. Sub elementos de una lista.
4. Otro elemento más.

...Es posible escribir más de una línea en un elemento de una lista, agregando al menos un espacio al comienzo de cada línea. Y dejando una fila en blanco.

...Otra ejemplo de texto como parte de un mismo elemento de la lista.

* Para listas con viñetas se pueden utilizar los asterístcos.
- O los signos menos.
+ O los signos más.
```

1. Primer elemento de una lista numerada.
2. Otro elemento.
  * Un elemento de una lista con viñetas.
1. El nro. utilizado no tiene importancia, será calculado de forma automática.
   1. Sub elementos de una lista.
4. Otro elemento más.

   Es posible escribir más de una línea en un elemento de una lista, agregando 3 espacios al comienzo de cada línea. Y dejando una fila en blanco.

   Otra ejemplo de texto como parte de un mismo elemento de la lista.

* Para listas con viñetas se pueden utilizar los asterístcos.
- O los signos menos.
+ O los signos más.

Enlaces
=======

Existen varias formas de crear un enlace.

```markdown
[El texto a mostrar en el enlace](https://www.google.com)

[El texto a mostrar en el enlace](https://www.google.com "El texto a mostrar cuando el mouse se pare sobre el enlace")

[Una referencia interna][Texto arbitrario sensible a mayúsculas/minúsculas]

[Un enlace relativo a una imagen o documento](imagen.jpg)

[Es posible utilizar números para referencias internas][1]

O simplemente escribir [la referencia al enlace].

Cualquier dirección Web serán traducida como un enlace externo. Por ej. https://google.com.ar
También si son escritas con símbolos mayor y menor: <https://google.com.ar>.

Los siguientes son los textos utilizados en las referencias internas.

[Texto arbitrario sensible a mayúsculas/minúsculas]: http://pragmatica.com.ar
[1]: https://google.com.ar
[la referencia al enlace]: http://google.com.ar
```

[El texto a mostrar en el enlace](https://www.google.com)

[El texto a mostrar en el enlace](https://www.google.com "El texto a mostrar cuando el mouse se pare sobre el enlace")

[Una referencia interna][Texto arbitrario sensible a mayúsculas/minúsculas]

[Un enlace relativo a una imagen o documento](imagen.jpg)

[Es posible utilizar números para referencias internas][1]

O simplemente escribir [la referencia al enlace].

Cualquier dirección Web serán traducida como un enlace externo. Por ej. https://google.com.ar
También si son escritas con símbolos mayor y menor: <https://google.com.ar>.

Los siguientes son los textos utilizados en las referencias internas.

[Texto arbitrario sensible a mayúsculas/minúsculas]: http://pragmatica.com.ar
[1]: https://google.com.ar
[la referencia al enlace]: http://google.com.ar

Imágenes
========

```markdown
Aquí se puede ver una imagen, incluso con un texto alternativo:

Estilo en-línea:
![Texto alternativo](http://pragmatica.com.ar/recursos/imagenes/logo-pragmatica.png "Texto a mostrar al pasar el mouse sobre la imagen")

Referenciando una imagen:
![Texto alternativo][logo-pragmatica]

[logo-pragmatica]: http://pragmatica.com.ar/recursos/imagenes/logo-pragmatica.png "Pragmática"
```

Aquí se puede ver una imagen, incluso con un texto alternativo:

Estilo en-línea:
![Texto alternativo](http://pragmatica.com.ar/recursos/imagenes/logo-pragmatica.png "Texto a mostrar al pasar el mouse sobre la imagen")

Referenciando una imagen:
![Texto alternativo][logo-pragmatica]

[logo-pragmatica]: http://pragmatica.com.ar/recursos/imagenes/logo-pragmatica.png "Pragmática"

Tablas
======

```markdown
El caracter dos puntos (:) es utilizado para definir la alineación de las columnas.

| Productos     | Detalles      |Importe|
| ------------- |:-------------:| -----:|
| Producto 1    | texto centrado| $10   |
| Producto 2    | ejemplo       | $100  |
| Producto 3    | otro ejemplo  | $1000 |

Los encabezados deben estar separados por una línea con al menos 3 guiones por celda. No es necesario alinear correctamente los caracteres "tubos" ( | ). Estos caracteres además son opcionales en los extremos.

Productos | Detalles | Importe
---|:---:| ---:
Producto 1 | centrado | $10
```

El caracter dos puntos (:) es utilizado para definir la alineación de las columnas.

| Productos     | Detalles      |Importe|
| ------------- |:-------------:| -----:|
| Producto 1    | texto centrado| $10   |
| Producto 2    | ejemplo       | $100  |
| Producto 3    | otro ejemplo  | $1000 |

Los encabezados deben estar separados por una línea con al menos 3 guiones por celda. No es necesario alinear correctamente los caracteres "tubos" ( | ). Estos caracteres además son opcionales en los extremos.

Productos | Detalles | Importe
---|:---:| ---:
Producto 1 | centrado | $10

Citas
=====

```markdown
> Texto de ejemplo para un bloque de cita.
> Esta línea pertenece al mismo bloque.

> Un ejemplo de cita **muy larga**: Lorem ipsum dolor sit amet consectetur adipisicing elit. Et repudiandae rem vel porro iusto similique ab vero dolor, minus blanditiis temporibus cumque consequatur corporis nulla autem enim sunt repellat consectetur.
```

> Texto de ejemplo para un bloque de cita.
> Esta línea pertenece al mismo bloque.

> Un ejemplo de cita **muy larga**: Lorem ipsum dolor sit amet consectetur adipisicing elit. Et repudiandae rem vel porro iusto similique ab vero dolor, minus blanditiis temporibus cumque consequatur corporis nulla autem enim sunt repellat consectetur.

Líneas separadoras
==================

```markdown
Tres (3) o más caracteres...

---

Guiones

***

Asterístcos

___

Guiones bajos
```

Tres (3) o más caracteres...

---

Guiones

***

Asterístcos

___

Guiones bajos

Párrafos
========

Básicamente todas las líneas que no cuenten con otra línea en blanco que las separe serán tomadas como parte de un mismo párrafo.

```markdown
Acá tiene una única línea para el párrafo.

Estas dos líneas comprenderán el mismo párrafo.
Ya que no cuentan con una línea en blanco que las separe.
```

Acá tiene una única línea para el párrafo.

Estas dos líneas comprenderán el mismo párrafo.
Ya que no cuentan con una línea en blanco que las separe.
