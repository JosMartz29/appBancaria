# appBancaria

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;;
}
/*Fuente de toda la ventana*/
  html {
    font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode',
     Geneva, Verdana, sans-serif;
  }

  .container {
    width: 100%;
    height: 100vh;
    background: #ffff;
    display: grid;
    grid-template-columns: repeat(7, 1fr);
    grid-auto-rows: minmax(100px, auto);
  }

  .lateral {
    background-color: #00abeb;
    display: grid;
    grid-column: 1 / 3;
    grid-template-rows: repeat(14, 1fr);
    grid-auto-rows: minmax(100px, auto);
  }

  .black_side {
    background-color: black;
    color: white;
    grid-row: 13 / 15;
  }

  .logo {
    grid-row: 4;
    margin: 3vw;
    width: 20vw;
  }

  .bienvenida {
    color: #ffff;
    grid-row: 5 / 7;
    margin: 3vw;
    width: 20vw;
    font-size: 90px;
    
  }

  /*
  .formulario {
    
  }

  .formulario::placeholder {
    color: black;
    padding: 50px;
  }
  
  .titulo {
    font-size: 40px;
    color: #00abeb;
  }
  
  span {
    color: black;
  }
  
  li {
    list-style-type: none;
    
  }

  .lista {
    line-height: 3;
  }

  input {
    background-color: #e7e7e7; 
    width: 200px;
    height: 25px;
    border: 0;
    border-radius: 8px;
    height: 40px;
    width: 435px;
    padding-left: 35px;
    margin-bottom: 10px;
  }
  
  .boton {
    background-color: black;
    color: white;
    align-items: center;
    border-radius: 32px;
    width: 130px;
    height: 38px;
  }
  
  
  
  .login {
    color: #00abeb;
  }
  */




  HTML
  <!DOCTYPE html>

<link rel="stylesheet" href="C:\Users\josmartinez\Documents\PANTALLAFIGMA\styles\styles.css" />
<html lang="es">
  
  <head>
		<meta charset="utf-8" />

		<div class="background">
      <title>Personal Banking | Crear Cuenta</title>
    </div>

	</head>
  
  <body>

    <section class="container">

      <section class="lateral">

        <div class="logo">
          <img src="../assets/logo_blanco.png" alt="logo_blanco">
        </div>

        <div class="bienvenida">
          <h1>Te damos la bienvenida al portal Personal Banking</h1>
        </div>

        <footer class="black_side">¿Ya tienes una cuenta? <a class="login" href="https://www.google.com">
          Iniciar sesión</a>
        </footer>
          
      </section>

      <form class="formulario">

          <!--<h1 class="titulo">Crear <span>Cuenta</span></h1>

          <input class="nombre" type="text" placeholder="Ingresa tus nombres" />

          <input type="text" placeholder="Ingresa tus apellidos" />

          <input type="text" placeholder="Ingresa tu DNI" />

          <input type="text" placeholder="Ingresa tu fecha de nacimiento" />

          <input type="password" placeholder="Ingresa tu nueva contraseña" />

          <input type="password" placeholder="Repite la contraseña que ingresaste" />

          <button type="submit" class="boton">Crear cuenta</button>-->

      </form>

    </section>
      
    
  </body>
