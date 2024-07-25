# desafio-vuex-tienda

## Videojuegos Vue.js con Vuex
Este proyecto es una aplicación de gestión de inventario de videojuegos, desarrollada con Vue.js y Vuex. La aplicación permite incrementar y decrementar el stock de cada videojuego.

## Características
Visualización de videojuegos: Muestra una lista de videojuegos con su código, nombre, stock y precio.
Incremento/Decremento de stock: Permite incrementar y decrementar el stock de cada videojuego mediante botones.

## Estructura del Proyecto
src/store/index.js: Archivo donde se configura Vuex, se define el estado global, las mutaciones y las acciones.
src/App.vue: Componente principal que muestra la lista de videojuegos y permite la modificación del stock.
## Uso
Visualizar videojuegos: La tabla en la página principal muestra la información de los videojuegos.
Modificar stock: Utiliza los botones "+" y "-" para incrementar o decrementar el stock de un videojuego.
Dependencias
Vue.js: Framework JavaScript utilizado para construir la interfaz de usuario.
Vuex: Librería de gestión de estado para aplicaciones Vue.js
## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
