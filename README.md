# <img align="left" alt="React" width="26px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/react/react.png" /> React guía básica
Comprende React JS

## ⚡ Resumen 🚀

00. Código inicial de copia y pega para el resto de ejercicios.
01. Creando una interfaz con Vanilla Javascript and DOM
- div root donde se almacenaran los elementos del DOM generados con javascript
- luego un script, guardaremos root, crearemos un nuevo div, y a ese elemento le establecemos un texto y una clase. Luego le añadimos a ese root el elemento.
02. User interface con React CreateElement API Explica la diferencia entre el código hecho puramente en js, con el de ahora puramente hecho con react. El resultado es el mismo. Vemos las props del elemento en un console.log y dentro de console props están las propiedades del elemento.
03. User interface con React JSX Sintaxis
Cuando usas jSX, la consola te da un error porque necesita ser compilado por BABEL para poder usar jsx
04. Usar JSX efectivo con React: Explica el significado de Children. puede interpolar valores con estas llaves colocando cualquier expresión entre llaves y hacer que esa expresión se transfiera a la API React.createElement. cambiamos container a not container... siempre coge lo último.
05. React Fragments, es para renderizar 2 elementos, uno al lado del otro y la manera simplificada de hacerlo, es abriendo y cerrando con <>...lololo....</>
06. Simple Reusable Componente de react. Aprendemos por qué las cosas funcionan de la manera en que lo hacen y cómo usar esto para su beneficio.
07. Validar con PropTypes. valida las propiedades que se le pasan a un componente. de aqui los famosos Proptypes.string.required que ya conoces. con isRequired, aparecen dos warning bien rojos en consola.. flipante.
08. Comprender la interpolación en JSX, digamos que es como saltamos en el código de jsx a string o a html como si nada. Es lo que hace.
09. CLOCK, todo el rato se renderiza, pero aprendemos a como evitarlo metiendo el codigo en una funcion y llamandolo con intervalo, setInterval(tick, 1000)
10. ¿porqué es className? aplicar estilos
11. Event Handlers: llamada a funcion que la ejecuta, es el tipico onClick={handleClick}
12. hook useState, guardar el estado
13. useEffect (localStorage) Quiero poder escribir aquí algún valor y guardarlo en localStorage para que cuando actualice la página, ese valor se recupere de localStorage y se cargue en la entrada.
14. "inicializador perezoso" con useState... En resumen, el problema que estamos resolviendo aquí es que la lectura en localStorage no es necesaria, excepto para la representación inicial de nuestro componente. Convertimos nuestro argumento de valor inicial aquí en una función para que React lo llame solo cuando sea necesario para obtener ese valor inicial, que está solo en el primer renderizado.
15. con useEffect puedes usar [x] como parámetro final. Asi, solo se actualizará cuando X cambie de estado.
En resumen, el problema que estábamos resolviendo aquí es que nuestra devolución de llamada de efecto se estaba llamando más de lo necesario. Quiero hacer una nota especial aquí, que solo porque se llamaba más de lo necesario no significaba que tuviéramos un error en nuestra aplicación, por lo que esto es solo una optimización para hacer que nuestra aplicación se ejecute un poco más rápido.
16. Ganchos personalizados reutilizables, FTI: ESTO ES PARA VERLO BIEN.
17. hook REFS
18.  Entender el flow de react hooks. useState siempre se lanza entre el inicio y el final del render mientras que useEffect siempre detrás.
19. FORM Para evitar el refresh completo de la página en formularios usamos event.preventDefault()
20. FORM Formularios dinámicos > ejemplo sencillo donde sabemos exactamente lo que escribe el usuario con onChange, cambiar el estado del componente, lanzar y mensaje de error y bloquear el boton de envio
21. FORM Es genial que podamos mostrar un mensaje de error si hay un carácter en mayúsculas y deshabilitamos el botón de envío, pero sería aún mejor si no permitiéramos que el usuario escribiera caracteres en mayúscula en primer lugar.
22. Boundaries React - recoge sobre todo errores de call-stack y necesitamos el paquete de npm para hacerlo mas sencillo, es para que te muestre errores, el ejemplo que muestra en la docu de react es brutal
23. Key prop para cuando hagas listas, siempre meterle una prop key={item.id}
24. ¿Como compartir el estado entre 2 componentes HERMANOS?, importante aprender como lift state up and push state back down, que es colocation en react
25. HTTP con react (fetch), USAREMOS use effect para que no se actualice nuestra aplicacion.
26. HTTP errores con react (pending, reject.. etc)
27. React Developer Tools
28. codesandbox github y netlify (esto es lo más)