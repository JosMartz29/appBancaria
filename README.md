# appBancaria

HTML:
<html lang="es">
<meta charset="UTF-8">
<link rel="stylesheet" href="styles.css"

<head>
    
    <title>Personal Banking | Crear Cuenta</title>
    
</head>

<!-- Contenedor Principal -->
<section class="container">

    <section class="lateral_banner"> <!-- Contenedor del banner celeste con el logo y la bienvenida de la pagina -->

        <img id="logo" src="white_logo.png" alt="white_logo">

        <h1 id="welcome">Te damos la bienvenida al portal Personal Banking</h1>

        <footer class="black_banner">
            <p id="question">¿Ya tienes una cuenta? <a id="login" href="https://www.google.com">Iniciar sesión</a></p>
        </footer>

    </section>

    <section class="form_base"> <!-- Contenedor del layout blanco donde se encuentra el título, el formulario y el botón -->

        <div id="form_title">
            <h1 id="titulo">Crear <span>Cuenta</span></h1>
        </div>

        <form id="formulario">
            <input type="text" placeholder="Ingresa tus nombres" />
      
            <input type="text" placeholder="Ingresa tus apellidos" />
      
            <input type="text" placeholder="Ingresa tu DNI" />
      
            <input type="text" placeholder="Ingresa tu fecha de nacimiento" />
      
            <input type="password" placeholder="Ingresa tu nueva contraseña" />
      
            <input type="password" placeholder="Repite la contraseña que ingresaste" />
        </form>

        <div class="form_button">
            <button type="submit" id="boton">Crear cuenta</button>
        </div>
    </section>
    
</section>



CSS:
* { 
    margin: 0; 
    padding: 0; 
    box-sizing: border-box; 
}

/*Fuente de toda la ventana*/ 
html { 
    font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif; 
}


/* Conteiner principal (base balnco) */
.container { 
    width: 100%; 
    height: 100vh;
    margin: 0;
    background: #ffff; 
    display: grid; 
    grid-template-columns: repeat(7, 1fr); 
    grid-auto-rows: minmax(100px, auto); 
}


/* Conteiner secundario (banner celeste) */
.lateral_banner { 
    background-color: #00abeb;
    display: grid;
    grid-column: 1 / 3;
    grid-template-rows: repeat(14, 1fr);
    grid-auto-rows: minmax(100px, auto); 
}

#logo /* logo de la compañia */ { 
    grid-row: 5;
    width: 170px;
    margin: 1.5vw;
    margin-bottom: 0;
}

#welcome /* texto dentro del banner celeste */ { 
    color: #ffff;
    grid-row: 6/7;
    margin: 1.5vw;
    margin-top: 1vw;
    font-size: 40px;
    width: 25vw;
}


/* Conteiner terciario (banner negro) */
.black_banner { 
    background-color: black;
    grid-row: 12 / 15;
    grid-auto-rows: minmax(100px, auto); 
}

#question /* texto dentro del banner negro */ {
    color: white;
    grid-row: 14;
    margin: 1.5vw;
    margin-top: 6vh;
}

#login /* enlace de login en el banner negro */ { 
    color: #00abeb; 
} 


/* Base 3x3 para colocar el formulario de registro centrado en el banner blanco */
.form_base {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-auto-columns: minmax(100px, auto);
    grid-template-rows: repeat(3, 1fr);
    grid-auto-rows: minmax(100px, auto);
    grid-column: 3 / 8;
}

#form_title /* contenedor para colocar el titulo en el banner blanco */ {
    grid-column: 2;
    grid-row: 1;
    margin-top: 20vh;
}

#titulo /* Titulo principal del formulario */ { 
    font-size: xxx-large;
    color: #00abeb;
    margin-bottom: 20px;
}

#formulario /* Contenedor para el Formulario */ {
    grid-column: 2;
    grid-row: 2;
    line-height: 3;
}

input { 
    background-color: #e7e7e7;
    border: 0;
    border-radius: 6px;
    height: 45px;
    width: 450px;
    padding-left: 35px;
    margin-bottom: 20px;
    font-size: medium;
}

span { 
    color: black; 
}

/* Posicionamiento del botón */ 
.form_button {
    grid-column: 2;
    grid-row: 3;
}

#boton { 
    background-color: black;
    color: white;
    font-weight: bold;
    font-size: medium;
    border-radius: 32px;
    width: 175px;
    height: 50px; 
}

#boton:active /* Trigger para cambiar el tamaña del boton */ {
    transform: scale(.9);
}

#boton:hover /* Trigger para cambiar el color cuando el cursor se posa en el boton */ {
    background-color: #00abeb;
    border: 0;
} 
