


<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Bienvenido a mi perfil de GitHub</title>
  <style>
      body {
          font-family: Arial, sans-serif;
          background-color: #f4f4f4;
          color: #333;
          text-align: center;
          padding: 50px;
      }
      h1 {
          color: #4CAF50;
      }
      button {
          padding: 10px 20px;
          font-size: 16px;
          cursor: pointer;
          background-color: #4CAF50;
          color: white;
          border: none;
          border-radius: 5px;
      }
      .info {
          display: none;
          margin-top: 20px;
          background-color: #e7f3fe;
          border-left: 6px solid #2196F3;
          padding: 10px;
      }
  </style>
</head>
<body>

  <h1 id="nombre">¡Hola, soy José Zuaga!</h1>
  <p id="descripcion">Soy desarrollador web.</p>
  <button onclick="toggleInfo()">Mostrar más sobre mí</button>
  
  <div class="info" id="extraInfo">
      <h2>Acerca de mí</h2>
      <p>Me gusta trabajar en proyectos de código abierto, aprender nuevas tecnologías y colaborar con otros desarrolladores.</p>
      <p>Habilidades: JavaScript, Python, React, Node.js, y más.</p>
  </div>

  <script>
      let isDeveloper = true;

      function toggleInfo() {
          var info = document.getElementById("extraInfo");
          info.style.display = (info.style.display === "none" || info.style.display === "") ? "block" : "none";

          // Cambiar el texto
          var nombre = document.getElementById("nombre");
          var descripcion = document.getElementById("descripcion");
          if (isDeveloper) {
              descripcion.innerText = "Soy José Zuaga.";
              nombre.innerText = "¡Hola, soy un desarrollador web!";
              isDeveloper = false;
          } else {
              descripcion.innerText = "Soy desarrollador web.";
              nombre.innerText = "¡Hola, soy José Zuaga!";
              isDeveloper = true;
          }
      }
  </script>

</body>
</html>

