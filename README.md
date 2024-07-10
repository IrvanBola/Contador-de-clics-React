<h1>Contador de Clics</h1>
    <p>Este proyecto es una aplicación simple de un contador de clics desarrollada con React. La aplicación permite al usuario incrementar y reiniciar el contador mediante botones.</p>
    
    <h2>Estructura del Proyecto</h2>
    <p>El proyecto está organizado en las siguientes carpetas y archivos:</p>
    <ul>
      <li><strong>src</strong>: La carpeta principal del código fuente.
        <ul>
          <li><strong>componentes</strong>: Contiene los componentes de React utilizados en la aplicación.
            <ul>
              <li><strong>Boton.jsx</strong>: Un componente de botón que puede actuar como un botón de clic o de reinicio basado en las propiedades (props) que recibe.</li>
              <li><strong>Contador.jsx</strong>: Un componente que muestra el número de clics.</li>
            </ul>
          </li>
          <li><strong>style-sheets</strong>: Contiene las hojas de estilo CSS utilizadas para dar estilo a los componentes.
            <ul>
              <li><strong>Boton.css</strong>: Estilos específicos para el componente de botón.</li>
              <li><strong>Contador.css</strong>: Estilos específicos para el componente de contador.</li>
            </ul>
          </li>
          <li><strong>App.css</strong>: La hoja de estilo principal para la aplicación.</li>
          <li><strong>App.jsx</strong>: El componente principal de la aplicación que maneja el estado del contador y renderiza los componentes <code>Contador</code> y <code>Boton</code>.</li>
          <li><strong>index.js</strong>: El punto de entrada principal de la aplicación React.</li>
        </ul>
      </li>
    </ul>
    
    <h2>Funcionalidad</h2>
    
    <h3>Componente <code>App</code></h3>
    <p>El componente principal que:</p>
    <ul>
      <li>Importa y aplica los estilos CSS.</li>
      <li>Utiliza el hook <code>useState</code> para manejar el estado del contador.</li>
      <li>Define dos funciones principales:
        <ul>
          <li><code>manejarClic</code>: Incrementa el número de clics en uno.</li>
          <li><code>reiniciarContador</code>: Restablece el número de clics a cero.</li>
        </ul>
      </li>
      <li>Renderiza el componente <code>Contador</code> y dos componentes <code>Boton</code> con diferentes props.</li>
    </ul>
    
    <h3>Componente <code>Contador</code></h3>
    <p>Un componente que:</p>
    <ul>
      <li>Recibe el número de clics como una prop.</li>
      <li>Muestra el número de clics en la pantalla.</li>
    </ul>
    
    <h3>Componente <code>Boton</code></h3>
    <p>Un componente que:</p>
    <ul>
      <li>Recibe tres props: <code>texto</code>, <code>esBotonDeClic</code>, y <code>manejarClic</code>.</li>
      <li>Muestra un botón cuyo estilo y función dependen de si es un botón de clic o de reinicio, según la prop <code>esBotonDeClic</code>.</li>
      <li>Llama a la función <code>manejarClic</code> cuando se hace clic en el botón.</li>
    </ul>
    
    <h2>Estilos CSS</h2>
    <ul>
      <li><strong>App.css</strong>: Establece el diseño general y la apariencia de la aplicación, incluyendo la disposición de los componentes y el color de fondo.</li>
      <li><strong>Boton.css</strong>: Define los estilos para los botones, incluyendo la apariencia de los botones de clic y de reinicio.</li>
      <li><strong>Contador.css</strong>: Define los estilos para el componente de contador, incluyendo el tamaño y la fuente del texto que muestra el número de clics.</li>
    </ul>
    
    <h2>Uso de Props</h2>
    <p>Los componentes <code>Boton</code> y <code>Contador</code> utilizan props para recibir datos y comportamientos desde el componente <code>App</code>:</p>
    <ul>
      <li><code>Contador</code> recibe una prop <code>numClics</code> para mostrar el número actual de clics.</li>
      <li><code>Boton</code> recibe:
        <ul>
          <li><code>texto</code>: El texto que se mostrará en el botón.</li>
          <li><code>esBotonDeClic</code>: Un booleano que determina si el botón es de clic o de reinicio.</li>
          <li><code>manejarClic</code>: La función que se ejecutará cuando el botón sea clicado.</li>
        </ul>
