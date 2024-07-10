# Contador de Clics

Este proyecto es una aplicación simple de un contador de clics desarrollada con React. La aplicación permite al usuario incrementar y reiniciar el contador mediante botones.

## Estructura del Proyecto

El proyecto está organizado en las siguientes carpetas y archivos:

- **src**: La carpeta principal del código fuente.
  - **componentes**: Contiene los componentes de React utilizados en la aplicación.
    - **Boton.jsx**: Un componente de botón que puede actuar como un botón de clic o de reinicio basado en las propiedades (props) que recibe.
    - **Contador.jsx**: Un componente que muestra el número de clics.
  - **style-sheets**: Contiene las hojas de estilo CSS utilizadas para dar estilo a los componentes.
    - **Boton.css**: Estilos específicos para el componente de botón.
    - **Contador.css**: Estilos específicos para el componente de contador.
  - **App.css**: La hoja de estilo principal para la aplicación.
  - **App.jsx**: El componente principal de la aplicación que maneja el estado del contador y renderiza los componentes `Contador` y `Boton`.
  - **index.js**: El punto de entrada principal de la aplicación React.

## Funcionalidad

### Componente `App`

El componente principal que:
- Importa y aplica los estilos CSS.
- Utiliza el hook `useState` para manejar el estado del contador.
- Define dos funciones principales:
  - `manejarClic`: Incrementa el número de clics en uno.
  - `reiniciarContador`: Restablece el número de clics a cero.
- Renderiza el componente `Contador` y dos componentes `Boton` con diferentes props.

### Componente `Contador`

Un componente que:
- Recibe el número de clics como una prop.
- Muestra el número de clics en la pantalla.

### Componente `Boton`

Un componente que:
- Recibe tres props: `texto`, `esBotonDeClic`, y `manejarClic`.
- Muestra un botón cuyo estilo y función dependen de si es un botón de clic o de reinicio, según la prop `esBotonDeClic`.
- Llama a la función `manejarClic` cuando se hace clic en el botón.

## Estilos CSS

- **App.css**: Establece el diseño general y la apariencia de la aplicación, incluyendo la disposición de los componentes y el color de fondo.
- **Boton.css**: Define los estilos para los botones, incluyendo la apariencia de los botones de clic y de reinicio.
- **Contador.css**: Define los estilos para el componente de contador, incluyendo el tamaño y la fuente del texto que muestra el número de clics.

## Uso de Props

Los componentes `Boton` y `Contador` utilizan props para recibir datos y comportamientos desde el componente `App`:
- `Contador` recibe una prop `numClics` para mostrar el número actual de clics.
- `Boton` recibe:
  - `texto`: El texto que se mostrará en el botón.
  - `esBotonDeClic`: Un booleano que determina si el botón es de clic o de reinicio.
  - `manejarClic`: La función que se ejecutará cuando el botón sea clicado.


 ![image](https://github.com/IrvanBola/Contador-de-clics-React/assets/122304883/8ebb37fb-3e97-400c-9da2-f7aa30db6959)

