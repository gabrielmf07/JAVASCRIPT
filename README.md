# Introducción a JavaScript

Este es un breve repaso sobre JavaScript, un lenguaje de programación de alto nivel ampliamente utilizado en el desarrollo web. JavaScript es conocido por ser un lenguaje versátil y flexible que permite la creación de aplicaciones interactivas y dinámicas en el lado del cliente.

## Tabla de contenidos

1. [¿Qué es JavaScript?](#qué-es-javascript)
2. [Variables y tipos de datos](#variables-y-tipos-de-datos)
3. [Estructuras de control](#estructuras-de-control)
4. [Funciones](#funciones)
5. [Objetos y arreglos](#objetos-y-arreglos)
6. [Manipulación del DOM](#manipulación-del-dom)
7. [Asincronismo y promesas](#asincronismo-y-promesas)
8. [Recursos adicionales](#recursos-adicionales)

## ¿Qué es JavaScript?

JavaScript es un lenguaje de programación de alto nivel, interpretado y orientado a objetos. Se utiliza principalmente en el desarrollo web para agregar interactividad y funcionalidad a las páginas web. JavaScript se ejecuta en el lado del cliente, lo que significa que se ejecuta en el navegador web del usuario final.

Además del desarrollo web, JavaScript también se utiliza en el desarrollo de aplicaciones móviles, servidores de backend (con Node.js), extensiones de navegador y más. JavaScript es un lenguaje de programación muy versátil que ha evolucionado y se ha vuelto fundamental en el desarrollo moderno.

## Variables y tipos de datos

En JavaScript, puedes declarar variables utilizando las palabras clave `var`, `let` o `const`. JavaScript es un lenguaje de tipado dinámico, lo que significa que no es necesario declarar explícitamente el tipo de una variable.

JavaScript admite varios tipos de datos, incluyendo:

- Números: enteros y decimales.
- Cadenas de texto: texto entre comillas.
- Booleanos: `true` o `false`.
- Objetos: estructuras de datos que agrupan propiedades y métodos.
- Arreglos: listas ordenadas de elementos.
- Null y undefined: valores especiales que representan la ausencia de un valor.

## Estructuras de control

JavaScript ofrece estructuras de control para controlar el flujo de ejecución de un programa. Algunas de las estructuras de control más comunes en JavaScript son:

- Declaraciones `if`, `else if` y `else`: permiten ejecutar bloques de código condicionalmente.
- Bucles `for`, `while` y `do...while`: permiten repetir bloques de código mientras se cumpla una condición.
- Sentencias `switch`: permiten tomar decisiones basadas en múltiples casos.

## Funciones

Las funciones en JavaScript son bloques de código reutilizables que se pueden invocar en cualquier momento. Puedes definir tus propias funciones utilizando la palabra clave `function`.

Las funciones pueden aceptar parámetros, que son valores que se pasan a la función cuando se invoca. Las funciones también pueden devolver un valor utilizando la palabra clave `return`.

Aquí hay un ejemplo básico de una función en JavaScript:

```javascript
function saludar(nombre) {
  console.log("Hola, " + nombre + "!");
}

saludar("Juan");
```

## Objetos y arreglos

En JavaScript, los objetos y los arreg

los son estructuras de datos fundamentales. Los objetos son estructuras que contienen propiedades y métodos, mientras que los arreglos son listas ordenadas de elementos.

Puedes crear objetos utilizando la sintaxis de llaves `{}` y acceder a las propiedades utilizando la notación de punto `objeto.propiedad`.

Los arreglos se crean utilizando la sintaxis de corchetes `[]` y puedes acceder a los elementos utilizando índices numéricos.

Aquí hay un ejemplo de un objeto y un arreglo en JavaScript:

```javascript
var persona = {
  nombre: "Juan",
  edad: 25,
  profesion: "Desarrollador"
};

var numeros = [1, 2, 3, 4, 5];
```

## Manipulación del DOM

El DOM (Document Object Model) es una representación en memoria de la estructura de un documento HTML. JavaScript proporciona métodos y propiedades para manipular y acceder a elementos del DOM.

Puedes utilizar JavaScript para seleccionar elementos del DOM, modificar su contenido, agregar o eliminar elementos y manejar eventos.

Aquí hay un ejemplo básico de manipulación del DOM en JavaScript:

```javascript
// Obtener un elemento del DOM por su ID
var elemento = document.getElementById("mi-elemento");

// Modificar el contenido de un elemento
elemento.textContent = "Nuevo contenido";

// Agregar un nuevo elemento al DOM
var nuevoElemento = document.createElement("p");
nuevoElemento.textContent = "Nuevo párrafo";
document.body.appendChild(nuevoElemento);

// Manejar un evento de clic
elemento.addEventListener("click", function() {
  console.log("Se hizo clic en el elemento");
});
```

## Asincronismo y promesas

JavaScript admite operaciones asincrónicas, como llamadas a API o carga de archivos, utilizando promesas. Las promesas son objetos que representan un valor que puede estar disponible ahora, en el futuro o nunca.

Puedes utilizar promesas para realizar tareas asincrónicas y manejar los resultados exitosos o errores de esas tareas.

Aquí hay un ejemplo básico de una promesa en JavaScript:

```javascript
function obtenerDatos() {
  return new Promise(function(resolve, reject) {
    // Simular una llamada asincrónica exitosa después de 2 segundos
    setTimeout(function() {
      resolve("Datos obtenidos");
    }, 2000);
  });
}

obtenerDatos()
  .then(function(datos) {
    console.log(datos);
  })
  .catch(function(error) {
    console.error(error);
  });
```

## Recursos adicionales

- [Documentación oficial de JavaScript en MDN](https://developer.mozilla.org/es/docs/Web/JavaScript): La documentación oficial de JavaScript en Mozilla Developer Network (MDN) es una excelente fuente de referencia para aprender más sobre el lenguaje y sus características.
- [JavaScript.info](https://javascript.info/): Un sitio web que ofrece tutoriales y recursos completos sobre JavaScript, desde los fundamentos hasta temas avanzados.
- [Eloquent JavaScript](https://eloquentjavascript.net/): Un libro en línea gratuito que cubre JavaScript de manera exhaustiva, adecuado tanto para principiantes como para programadores con experiencia.

Este repaso solo cubre los conceptos básicos de JavaScript. JavaScript es un lenguaje poderoso y versátil con muchas características y funcionalidades avanzadas. A medida que profundices en tu aprendizaje de JavaScript, podrás explorar temas como programación orientada a objetos, módulos, asincron

ismo avanzado y más.
