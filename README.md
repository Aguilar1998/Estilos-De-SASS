## Install Node

https://nodejs.org/en

# SASS:

- Variables
- Mixins
- Mixins como Neomorfismo, Flex o Media
- Crea tu propio Mixin
- Anidación y Selector &

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
