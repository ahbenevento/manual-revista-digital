# Cómo publicar notas

## Título

Cada publicación deberá tener al menos un **título principal**, definido por un caracter numeral (#).

Este título será utilizado también para la portada, listas e incluso en los resultados de una búsqueda.

```markdown
# Hasta Clarín no paro
```

Es recomendable, pero no necesario, que solo se defina un único título de nivel principal (o nivel 1). El resto deberían ser subtítulos y comenzar con la menos dos caracteres numeral.

```markdown
## Subtítulo de nivel 2

### Subtítulo de nivel 3
```

## Imágenes

El Bot permitirá subir imágenes para cualquier contenido, incluso mucho antes de publicarlo.

Es recomendable que por cada imagen se defina al menos un **título u observación** sobre la misma. Además  podrá definir un resumen o detalle sobre el contexto de la fotografía.

Solo en el caso de utilizar imágenes de otros sitios Web será necesario agregar un texto alternativo, que será utilizado de igual forma a lo comentado más arriba.

```markdown
(imagen-previamente-subida.jpg)

(http://pragmatica.com.ar/recursos/imagenes/logo-pragmatica.png "Título o descripción de la imagen externa")
```

> En las imágenes subidas mediante el Bot solo será necesario escribir el nombre del archivo sin dirección Web.

## Metadatos

Según sea necesario un archivo podrá tener un bloque de información adicional, o metadatos, que el Bot deberá interpretar.

Un bloque de metadatos deberá estar definido por dos líneas de inicio y fin, con al menos 3 signos igual (=).

```
===

...bloque para metadatos...

===
```

La forma en que se define cada uno de los datos dentro del bloque es iniciando cada línea con una **"palabra clave"** seguida de la información específica.

### Resumen de las palabras claves disponibles

+ **autor**

    El **alias** de cada uno de los autores de la nota. Cada autor deberá estar previamente registrado en la base de datos.

+ **etiqueta**

    Cada una de las etiquetas definidas para la publicación.

+ **prefacio**

    El texto introductorio a la publicación. Dependiendo del diseño, puede ser utilizado dentro de la publicación, en resultados de búsqueda, metadatos para buscadores e incluso en la portada de la revista.

+ **tipo**

    Permite indicar el tipo de contenido a publicar: **nota** (predeterminado), **ensayo**, **opinión**, etc.

+ **estado**

    Permite indicar en qué estado debe guardarse el contenido: `borrador`, `revisar`, `oculto`.

### Palabras claves

#### **autor**

El **alias** de cada uno de los autores de la nota. Cada autor deberá estar previamente registrado en la base de datos.

Esto es opcional si el usuario es el autor pero requerido si la publicación tiene más de una autoría. O bien cuando el autor de la nota no es el usuario que sube el archivo.

```
1. Varios autores:

===
autor juan
autor guri
===

2. En una misma línea (separados por comas):

===
autor juan, guri
===

3. Definiendo roles:

===
autor guri
autor faca Ilustraciones
===
```

#### **etiqueta**

Cada una de las etiquetas definidas para la publicación. Si especifica más de una por línea deberá separarlas con espacios.

Si la etiqueta posee dos o más palabras deberá encerrarse entre comillas simples ('') o dobles ("").

```
1. Varias etiquetas:

===
etiqueta uno
etiqueta dos
etiqueta tres
===

2. En una misma línea (separados por espacios):

===
etiqueta uno dos tres
===

3. Etiquetas con más de una palabra:

===
etiqueta "Esto es solo una prueba" prueba
===
```

#### **prefacio**

El texto introductorio a la publicación. Dependiendo del diseño, puede ser utilizado dentro de la publicación, en resultados de búsqueda, metadatos para buscadores e incluso en la portada de la revista.

```
1. Como en el resto de las palabras claves puede escribirse todo en una misma línea:

===
prefacio Lorem ipsum dolor sit amet, consectetur adipisicing elit. Iure consectetur optio doloremque, in repellendus nulla inventore officia at ducimus modi. Suscipit accusantium qui dolores eligendi quidem maxime blanditiis repellendus. Repellat.
===

2. O bien definirse en varias llamadas:

===
prefacio Lorem ipsum dolor sit amet, consectetur adipisicing elit.
prefacio Iure consectetur optio doloremque, in repellendus nulla inventore officia at ducimus modi.
prefacio Suscipit accusantium qui dolores eligendi quidem maxime blanditiis repellendus. Repellat.
===

3. Incluso es posible incluir contenido Markdown:

===
prefacio **Escribiendo en negritas**
===
```

#### **tipo**

Permite indicar el tipo de contenido a publicar. Estos tipos no pueden agregarse o modificarse mediante el Bot y cualquier cambio deberá solicitarse de forma explícita.

Tipo de contenido | Alias utilizado en el Bot
----------------- | -------------------------
**Nota** (predeterminado) | `nota`
**Ensayo** | `ensayo`
**Opinión** | `opinion`

<br>

#### **estado**

Permite indicar en qué estado debe guardarse el contenido.

Alias utilizado en el Bot | Detalles del estado
------------------------- | -------------------
`borrador` | Este estado permite subir el contenido sin notificar a otros autores.
`revisar` | **En revisión**, el Bot notificará que el contenido debe confirmarse. A menos que se indique otro valor, este estado es el predeterminado para los contenidos nuevos.
`oculto` | En este  estado el artículo se publica sin visualizarse en la portada, listados o resultados de búsqueda.

### Ejemplos (combinando palabras claves)

```
===
autor guri, faca Ilustraciones
etiqueta "Algo para mostrar"
prefacio Sueñan las pulgas con comprarse un perro...
tipo ensayo
estado borrador
===
```

```
===
autor guri
autor juan
etiqueta "Diego Maradona" d10s
===
```

```
===
etiqueta locales
tipo opinion
estado oculto
===
```
