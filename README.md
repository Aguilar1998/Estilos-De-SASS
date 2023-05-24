## Install Node

https://nodejs.org/en

Antes de continuar, realiza un backup de tus archivos CSS, ya que se sobre escribirán cuando empieces a usar SASS.

![Imagen del proyecto](https://github.com/eduardofierropro/SASS-y-SCSS-Aumenta-tu-nivel-como-Frontend/blob/main/assets/home1.png)

# SASS: Mixins, variables, Nesting Flex, Grid y Media Queries

- Variables
- Mixins
- Mixins como Neomorfismo, Flex o Media
- Crea tu propio Mixin
- Anidación y Selector &

[![Youtube](https://img.shields.io/static/v1?label=&message=ver%20playlist&color=FF0000&logo=youtube&logoColor=white&style=for-the-badge)](https://www.youtube.com/watch?v=-VJfeNL-VH0&list=PLJpymL0goBgFAUYDei7CoJCiHjcmgioUt)

## 👉🏽 Para descargar este proyecto::

```
 git clone https://github.com/Aguilar1998/Herramientas-De-SASS.git
 cd Herramientas-De-SASS
 git i

```

## 👉🏽 Forma de instalar Sass al momento de crear un proyecto desde cero:

```
    npm init
    npm install -D node-sass nodemon
```

### Crear la carpeta scss y css con sus archivos respectivos .

### Incluir los siguientes script dentro de packaje.json

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

### Live SASS Compiler (extension de visual estudio code)
