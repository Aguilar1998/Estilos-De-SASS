Install Node

Antes de continuar, realiza un backup de tus archivos CSS, ya que se sobre escribirán cuando empieces a usar SASS.

![Imagen del proyecto](https://github.com/eduardofierropro/SASS-y-SCSS-Aumenta-tu-nivel-como-Frontend/blob/main/assets/home1.png)

# SASS: Mixins, variables, Nesting Flex, Grid y Media Queries

- Variables
- Mixins
- Mixins como Neomorfismo, Flex o Media
- Crea tu propio Mixin
- Anidación y Selector &

[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20playlist&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://www.youtube.com/watch?v=-VJfeNL-VH0&list=PLJpymL0goBgFAUYDei7CoJCiHjcmgioUt)

## Todos los vídeos de SASS

| Nombre                         | Youtube                                                                                                                                                               |
| ------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Variables en SASS              | [![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/eoAwVWeQf6U) |
| Mixins en SASS                 | [![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/-VJfeNL-VH0) |
| Mixins MUY ÚTILES en SASS      | [![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/h3yS1RuIKz4) |
| Crea tu propio Mixin en SASS   | [![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/56QVDvj9dHw) |
| Anidación y Selector & en SASS | [![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/56QVDvj9dHw) |

<!-- ## 👨🏻‍🏫 Apuntes de SASS

### ¿Qué es Sass vs CSS?
* CSS nos permite aplicar estilo al HTML
* SASS es un lenguaje que se convierte (compila) en CSS
* SCSS es un lenguaje que se convierte (compila) en CSS

Por lo tanto... ¿qué se entiende cuando decimos Sass?: **SASS es un lenguaje que se convierte *(compila)* en CSS**

### ¿Cómo se usa Sass?
Creas un archivo de SASS y lo conviertes *(compilas)* con herramientas.

### ¿Cómo se puede compilar Sass?
Puedes hacerlo de múltiples formas:

* Herramientas como Prepros 🚨 MUY FÁCIL 👉 [https://youtu.be/tArtLYlq9ws](https://youtu.be/tArtLYlq9ws)
* Consola con NodeJS
* Sistemas de Bundling como Webpack
* Sistemas de Task Runner como Grunt

#### ¿Cómo escribir variables en SASS?
Recuerda que :
* Declaramos(creamos) la variable
* Usamos la variable

>    🚨 Puedes ponerle el nombre que quieras pero usa "snake-case"
>
>    🚨 Si no sabes de nomenclaturas 👉 https://youtu.be/lhEJkeCJ3As


```scss

$negro : red; // Declaramos la variable

a{
    color: $negro; // 👈 Usamos la variable en una propiedad
}
p{
    background-color: $negro; // 👈 Usamos la variable en una propiedad
}
```

### ¿Qué pasa si tengo muchas variables?

```scss
$color-negro    : black;
$color-blanco   : white;
$fuente-normal  : Verdana;
$fuente-titulo  : Helvetica;
/* 👆 Aquí tenemos muchas variables y tenemos que repetir "color-", "fuente-" */

header{
    color       : $color-negro ;
    font-family   : $fuente-normal;
}
h1{
    background  : $color-blanco;
    font-family   : $fuente-titulo;
}
```

Vamos a ser organizados y guardar todas las variables en una lista de variables.
* Una lista de variables es un Array.
* Usaremos map-get() para usar las variables
```scss
$colores: (
    "negro"  : black,
    "blanco" : white,
);
$fuentes : (
    "normal"  : Verdana,
    "titulo" : Helvetica
);

header{
    color         : map-get( $colores , "negro"  ) ;
    font-family   : map-get( $fuentes , "normal" ) ;
}
h1{
    background    : map-get( $colores , "blanco" ) ;
    font-family   : map-get( $fuentes , "titulo" ) ;
}

```

<!--
## 🔴 Vídeos relacionados con las metodologías

| Nombre | Youtube |
|--|--|
|Reset CSS: Teoría|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/bXqPNoYFK8w)|
|Reset PRO: Código|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/Foieq2jTajE)|
|Nomenclaturas CSS|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/lhEJkeCJ3As)|
|Metodologías CSS|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/f0LpZoyY1gE)|
|Arquitecturas CSS|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/tUldrlfIGb4)|
|Cómo aplicar BEM en HTML y CSS|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/NucZM0GMRi4)|
|Cómo aplicar SUITCSS en HTML y CSS|[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20video&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/Vdmof9VSiEo)| -->

## 👉🏽 Forma de instalar Sass al momento de crear un proyecto desde cero:

```
    npm init
    npm install -D node-sass nodemon
```

## Crear la carpeta scss y css con sus archivos respectivos .

## Incluir los siguientes script dentro de packaje.json

```
    “build-css“: node-sass --include-path scss sass/style.scss css/main.css”,

    “watch-css“: “nodemon -e scss -x \”npm run build-css\””
```

```
    npm run watch-css
```

## 👉🏽 Forma corta de instalar Sass al momento de crear un proyecto desde cero:

```
    npm init

    npm install -g sass

    sass --watch scss:css
```

## Live SASS Compiler (extension de visual estudio code)
