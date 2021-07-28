# sala_gamer 
import { useState } from "react";



import ReactDOM from "react-dom";

import "./styles.css";


function App() {


var [nombre, setNome] = useState("");

var [contrasena, setData] = useState("");


function cambiar(URL) {


console.log("Nombre", nombre);


console.log("contraseña:", contrasena);


window.open("https://7dn0c.csb.app/");


}


return (


<div>


<h1>Formulario</h1>

<p>

USUARIO:

<input

placeholder="Usuario "

onChange={(evt) => setNome(evt.target.value)}
/>

</p>


<p>


CONTRASEÑA :


<input


placeholder="contraseña "

onChange={(evt) => setData(evt.target.value)}

/>
</p>

<button onClick={cambiar}>REGISTRO </button>



</div>



);


}

const rootElement = document.getElementById("root");


ReactDOM.render(<App />, rootElement);
