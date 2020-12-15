<template>
  <!DOCTYPE html>
  <html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BilleterApp</title>
  </head>
  <body>
 <div class="login" id= "login">
  <div class= "Titulo">
    <h1>Billeter<span>App</span></h1>
    <h2>Ingresar</h2>
    <form action="">
      <label for="Usuario"> Usuario</label>
      <input type="text" placeholder="Usuario">
      <label for="Contrasena"> Contraseña </label>
      <input type="password" placeholder="Contraseña">
      <button class="boton" type="button">Ingresar</button> <br> <br>
      <a href="#">¿Ha olvidado su contraseña?</a> <br>
      <a v-on:click="mostrarRegistro();">Registrarse</a>
    </form>
  </div>
 </div>

 <div> <v-if> </v-if>
 <div class="registrar" id= "registrar"> 
  <div class= "Titulo">
    <h1>Billeter<span>App</span></h1>
    <h2>Ingresar</h2>
    <form action="">
      <label for="Nombre"> Nombre</label>
      <input type="text" placeholder="Nombre">
      <label for="Usuario"> Usuario</label>
      <input type="text" placeholder="Usuario">
      <label for="Contrasena">Contraseña </label>
      <input type="password" placeholder="Contraseña">
      <label for="email">Email</label>
      <input type="email" placeholder="email">
      <label for="edad"> Edad</label>
      <input type="number" placeholder="edad">
      <label for="cedula">Cédula</label>
      <input type="number" placeholder="cedula">
      <button class="boton" type="button">Ingresar</button> <br> <br>
      <a href="#">¿Ha olvidado su contraseña?</a> <br>
      <a href="#">Registrarse</a>
    </form>
  </div>
 </div>
</div>
  </body>
  </html>
    
</template>


<script>
    export default {
    name: 'App',
    }
</script>

<script type= "text/javascript">
    function mostrarRegistro(){
      document.getElementById('login').style.display='none';
      document.getElementById('registrar').style.display='block';
    }
</script>




<style>
  body{
    font-family: sans-serif;
  }

  .Titulo span{
   color: #1dc4e7;
  }

  .login{
    width: 320px;
    height: 500px;
    background: rgba(0,0,0,0.6);
    color: white;
    top: 50%;
    left: 50%;
    position: absolute;
    transform: translate(-50%, -50%);
    box-sizing: border-box;
    padding: 60px 40px;
  }
  
  .login h1{
   margin: 0%;
   color: white;
   font-weight: 400;
   font-size: 30px;
   text-align: center;
  }

  .login h2{
    font-weight: 400;
    margin: 0%;
    margin-top: 30px;
    padding: 0 0 20px;
    display: block;
    font-size: 22px ;
    text-align: center;
  }

  .login label{
   font-weight: bold;
   margin: 0%;
   padding: 0;
   display: block;
   margin-top: 26px;
  }

  .login input[type="text"], .login input[type="password"]{
    border: none;
    border-bottom: 1px solid white;
    background: transparent;
    outline: none;  
    height: 40px; 
    color: white;
    font-size: 18px; 
  }

  .login .boton{
    border: 1px solid white;
    outline: none;
    height: 40px;
    color: white;
    background-color: #2190a7;
    font-size: 18px; 
    border-radius: 10px;
    width: 170px;
    line-height: 10px;
    margin-top: 40px;
    align-items: center;
    margin-left: 15%;
  } 

  .login .boton:hover{
    background-color: #0daccc;
    cursor: pointer;
  }

  .login a{
    text-decoration: none;
    font-size: 14px;
    color: white;
    line-height: 20px;
  }

  .login a:hover{
    color: darkgrey;
    cursor: pointer;
  }

  .registrar{
    width: 320px;
    height: 500px;
    background: rgba(0,0,0,0.6);
    color: white;
    top: 50%;
    left: 50%;
    position: absolute;
    transform: translate(-50%, -50%);
    box-sizing: border-box;
    padding: 60px 40px;
  }
  
  .registrar h1{
   margin: 0%;
   color: white;
   font-weight: 400;
   font-size: 30px;
   text-align: center;
  }

  .registrar h2{
    font-weight: 400;
    margin: 0%;
    margin-top: 30px;
    padding: 0 0 20px;
    display: block;
    font-size: 22px ;
    text-align: center;
  }

  .registrar label{
   font-weight: bold;
   margin: 0%;
   padding: 0;
   display: block;
   margin-top: 26px;
  }

  .registrar input[type="text"], .registrar input[type="password"]{
    border: none;
    border-bottom: 1px solid white;
    background: transparent;
    outline: none;  
    height: 40px; 
    color: white;
    font-size: 18px; 
  }

  .registrar .boton{
    border: 1px solid white;
    outline: none;
    height: 40px;
    color: white;
    background-color: #2190a7;
    font-size: 18px; 
    border-radius: 10px;
    width: 170px;
    line-height: 10px;
    margin-top: 40px;
    align-items: center;
    margin-left: 15%;
  } 

  .registrar .boton:hover{
    background-color: #0daccc;
    cursor: pointer;
  }

  .registrar a{
    text-decoration: none;
    font-size: 14px;
    color: white;
    line-height: 20px;
  }

  .registrar a:hover{
    color: darkgrey;
    cursor: pointer;
  }

  #registrar {
    display: none;

  }



</style>
