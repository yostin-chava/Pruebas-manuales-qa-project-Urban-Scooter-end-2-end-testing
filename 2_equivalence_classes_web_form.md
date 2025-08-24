# Clases de equivalencia y los valores límite para los campos de entrada .

<table>
  <tr>
    <th>Campo</th>
    <th>Nombre de la clase</th>
    <th>Límites</th>
    <th>Datos de prueba dentro de la clase</th>
    <th>Datos de prueba en los límites</th>
    <th>Explicación</th>
    <th>Estado</th>
    <th>Enlace al informe de errores</th>
    <th>Comentario</th>
  </tr>
  <!-- Nombre -->
  <!--  -->
  <tr>
    <td rowspan="13">Nombre</td>
    <td rowspan="2">Longitud del texto de 0 a 1 carácter</td>
    <td rowspan="2">0-1</td>
    <td rowspan="2"></td>
    <td>0 -> String vacio</td>
    <td>Límite inferior</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>1 -> A</td>
    <td>Límite superior</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td rowspan="4">Longitud del texto de 2 a 15 caracteres</td>
    <td rowspan="4">2-15</td>
    <td rowspan="4">11 -> Albert Eins</td>
    <td>2 -> Al</td>
    <td>Límite inferior</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>15 ->Albert Einstein</td>
    <td>Límite superior</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>3-> Alb</td>
    <td>Límite inferior + 1</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>14-> Albert Einstei</td>
    <td>Límite superior - 1</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td rowspan="2">Longitud del texto de 16 a más caracteres</td>
    <td rowspan="2">16 - +oo</td>
    <td rowspan="2">20 -> Albert Einsteinnnnnn</td>
    <td>16-> Albert Einsteinn</td>
    <td>Límite inferior y espacio en medio del texto</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>17-> Albert Einsteinnn</td>
    <td>Límite inferior + 1</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Espacio al inicio</td>
    <td></td>
    <td>_Alb</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Espacio al final</td>
    <td></td>
    <td>Alb_</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Guiones</td>
    <td></td>
    <td>Albert-Einstein</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Otros caracteres</td>
    <td></td>
    <td>@|b3rt .$%&.</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Caracteres de otro idioma</td>
    <td></td>
    <td>山姆</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  
  <!-- ---------- -->
  <!-- Intermedio -->
  <tr>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <!-- ---------- -->
  <!-- ---------- -->
  
  <!-- Apellido -->
  <!--  -->
  <tr>
    <td rowspan="13">Apellido</td>
    <td rowspan="2">Longitud del texto de 0 a 1 carácter</td>
    <td rowspan="2">0-1</td>
    <td rowspan="2"></td>
    <td>0 -> String vacio</td>
    <td>Límite inferior</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>1 -> A</td>
    <td>Límite superior</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td rowspan="4">Longitud del texto de 2 a 15 caracteres</td>
    <td rowspan="4">2-15</td>
    <td rowspan="4">11 -> Albert Eins</td>
    <td>2 -> Al</td>
    <td>Límite inferior</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>15 ->Albert Einstein</td>
    <td>Límite superior</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>3-> Alb</td>
    <td>Límite inferior + 1</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>14-> Albert Einstei</td>
    <td>Límite superior - 1</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td rowspan="2">Longitud del texto de 16 a más caracteres</td>
    <td rowspan="2">16 - +oo</td>
    <td rowspan="2">20 -> Albert Einsteinnnnnn</td>
    <td>16-> Albert Einsteinn</td>
    <td>Límite inferior y espacio en medio del texto</td>
    <td>NO APROBADO</td>
    <td><a href="https://yostinch.atlassian.net/browse/IEPF-8?atlOrigin=eyJpIjoiZWQxZTdhY2FjZGRhNDUwMWI5OTI3OTFhMzdmNzYxZGIiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>17-> Albert Einsteinnn</td>
    <td>Límite inferior + 1</td>
    <td>OMITIDA</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Espacio al inicio</td>
    <td></td>
    <td>_Alb</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Espacio al final</td>
    <td></td>
    <td>Alb_</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Guiones</td>
    <td></td>
    <td>Albert-Einstein</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Otros caracteres</td>
    <td></td>
    <td>@|b3rt .$%&.</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Caracteres de otro idioma</td>
    <td></td>
    <td>山姆</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>

  <!-- ---------- -->
  <!-- Intermedio -->
  <tr>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <!-- ---------- -->
  <!-- ---------- -->

  <!-- Direccion -->
  <!--  -->
  <tr>
    <td rowspan="16">Dirección</td>
    <td rowspan="4">Longitud del texto de 0 a 4 caracteres</td>
    <td rowspan="4">0-4</td>
    <td rowspan="4"></td>
    <td>0 -> String vacio</td>
    <td>Límite inferior</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>4 -> 1 Ma</td>
    <td>Límite superior</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>1 -> 1</td>
    <td>Límite inferior + 1</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>3 -> 1 M</td>
    <td>Límite superior - 1</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td rowspan="4">Longitud del texto de 5 a 50 caracteres</td>
    <td rowspan="4">2-15</td>
    <td rowspan="4">45 -> 1234 Main St, near Pico Station, East Los, CA</td>
    <td>5 -> 1 Mai</td>
    <td>Límite inferior</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>50-> 1 Main St, near Pico Station, East Los Angeles, CA</td>
    <td>Límite superior</td>
    <td>NO APROBADO</td>
    <td><a href="https://yostinch.atlassian.net/browse/IEPF-9?atlOrigin=eyJpIjoiNjlkM2EyOWZlYzgxNGZhODgyN2UyYTY1ZmJiNWFlZjMiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>6 -> 1 Main</td>
    <td>Límite inferior + 1</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>49-> 1 Main S, near Pico Station, East Los Angeles, CA</td>
    <td>Límite superior - 1</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td rowspan="2">Longitud del texto de 51 a más caracteres</td>
    <td rowspan="2">51 - +oo</td>
    <td rowspan="2">53 -> 1234 Main St, near Pico Station, East Los Angeles, CA</td>
    <td>51-> 12 Main St, near Pico Station, East Los Angeles, CA</td>
    <td>Límite inferior y espacio en medio del texto</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>52-> 123 Main St, near Pico Station, East Los Angeles, CA</td>
    <td>Límite inferior + 1</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Espacio al inicio</td>
    <td></td>
    <td>_1 Main</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Espacio al final</td>
    <td></td>
    <td>1 Main_</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Guiones</td>
    <td></td>
    <td>1-Main</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Puntos</td>
    <td></td>
    <td>12.Main.</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Otros caracteres</td>
    <td></td>
    <td>@|b3rt $%&</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Caracteres de otro idioma</td>
    <td></td>
    <td>阿爾伯特愛因斯坦</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>

  <!-- ---------- -->
  <!-- Intermedio -->
  <tr>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <!-- ---------- -->
  <!-- ---------- -->

  <!-- Estacion de metro -->
  <!--  -->
  <tr>
    <td rowspan="2">Estación de metro</td>
    <td>Estación de metro válida en la lista del backend</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>Estación de metro no válida en la lista del backend</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>

   <!-- ---------- -->
  <!-- Intermedio -->
  <tr>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <!-- ---------- -->
  <!-- ---------- -->

  <!-- Telefono -->
  <!--  -->
  <tr>
    <td rowspan="13">Teléfono</td>
    <td rowspan="4">Longitud de texto de 0 a 9 números</td>
    <td rowspan="4">0-9</td>
    <td rowspan="4">7 -> +1234567</td>
    <td>0 -> String vacio</td>
    <td>Límite inferior</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>9 -> +123456789</td>
    <td>Límite superior</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>1 -> +1</td>
    <td>Límite inferior + 1</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>8 -> +12345678</td>
    <td>Límite superior - 1</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td rowspan="3">Longitud de texto de 10 a 12 números</td>
    <td rowspan="3">10-12</td>
    <td rowspan="3"></td>
    <td>10 -> +1234567890</td>
    <td>Límite inferior</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>12 -> +123456789012</td>
    <td>Límite superior</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>11 -> +12345678901</td>
    <td>Límite inferior + 1 o Límite superior - 1</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td rowspan="2">Longitud de texto de 13 a más números</td>
    <td rowspan="2">13 - +oo</td>
    <td rowspan="2">17 -> +12345678901234567</td>
    <td>13 -> +1234567890123</td>
    <td>Límite inferior</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>14 -> +12345678901234</td>
    <td>Límite inferior + 1</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Simbolo +</td>
    <td></td>
    <td>+1234</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Número con espacio</td>
    <td></td>
    <td>1234 567890</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Otros caracteres</td>
    <td></td>
    <td>1234567/*-.</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Caracteres latinos</td>
    <td></td>
    <td>1234djshsd</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>

  <!-- ---------- -->
  <!-- Intermedio -->
  <tr>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <!-- ---------- -->
  <!-- ---------- -->

  <!-- Cuando entregar el scooter -->
  <!--  -->
  <tr>
    <td rowspan="3">Cuando entregar el scooter</td>
    <td>Fecha: un día después de realizar el pedido</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>Fecha: el mismo día de realizar el pedido</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td>NO APROBADO</td>
    <td><a href="https://yostinch.atlassian.net/browse/IEPF-10?atlOrigin=eyJpIjoiOWFlOWFmMDEwNWZlNGIwZWIxMGVmMTNiOTgzMGJjYTciLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>Fecha: un día antes de realizar el pedido</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td>NO APROBADO</td>
    <td><a href="https://yostinch.atlassian.net/browse/IEPF-11?atlOrigin=eyJpIjoiNDI2N2Q4M2M4MDIyNGNlZGE3ZTI0MzBiZTVhYjI0NmYiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>

  <!-- ---------- -->
  <!-- Intermedio -->
  <tr>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <!-- ---------- -->
  <!-- ---------- -->

  <!-- Periodo de alquiler -->
  <!--  -->
  <tr>
    <td>Periodo de alquiler</td>
    <td>Valor dentro de la lista desplegable</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>

  <!-- ---------- -->
  <!-- Intermedio -->
  <tr>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <!-- ---------- -->
  <!-- ---------- -->

  <!-- Color del scooter -->
  <!--  -->
  <tr>
    <td rowspan="2">Color del scooter</td>
    <td>Seleccionar 1 color</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>Seleccionar 2 colores</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>

  <!-- ---------- -->
  <!-- Intermedio -->
  <tr>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <!-- ---------- -->
  <!-- ---------- -->

  <!-- comentario -->
  <!--  -->
  <tr>
    <td rowspan="13">Comentario</td>
    <td rowspan="4">Longitud de texto de 0 a 24 caracteres</td>
    <td rowspan="4">0-24</td>
    <td rowspan="4">19 -> Hola muchas gracias</td>
    <td>0 -> String vacio</td>
    <td>Límite inferior</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>24 -> Hola muchas gracias atte</td>
    <td>Límite superior y espacio en medio</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>1 -> H</td>
    <td>Límite inferior + 1</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <tr>
    <td>23 -> Hola muchas gracias att</td>
    <td>Límite superior - 1</td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td rowspan="2">Longitud del texto de 25 a más caracteres</td>
    <td rowspan="2">25 - +oo</td>
    <td rowspan="2">29 -> Hola muchas gracias atte12345 </td>
    <td>25-> Hola muchas gracias att12</td>
    <td>Límite inferior y se evalua números</td>
    <td>NO APROBADO</td>
    <td><a href="https://yostinch.atlassian.net/browse/IEPF-12?atlOrigin=eyJpIjoiYzE1YzRmMDUxYjMyNGNjNmFiZWZlZTczMWQzNTMzNzYiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>26-> Hola muchas gracias att123</td>
    <td>Límite inferior + 1</td>
    <td>OMITIDA</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Espacio al inicio</td>
    <td></td>
    <td>_hola</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Espacio al final</td>
    <td></td>
    <td>hola_</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Guiones</td>
    <td></td>
    <td>hola-hola</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Puntos</td>
    <td></td>
    <td>hola.</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Comas</td>
    <td></td>
    <td>hola,</td>
    <td></td>
    <td></td>
    <td>APROBADO</td>
    <td></td>
  </tr>
  <!--  -->
  <tr>
    <td>Otros caracteres</td>
    <td></td>
    <td>@$%&</td>
    <td></td>
    <td></td>
    <td>NO APROBADO</td>
    <td><a href="https://yostinch.atlassian.net/browse/IEPF-13?atlOrigin=eyJpIjoiZDAxNzRhNWI5ZjBkNDZiODhlZWEwZTIwNTIyNTEwNWUiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <!--  -->
  <tr>
    <td>Caracteres de otro idioma</td>
    <td></td>
    <td>你好</td>
    <td></td>
    <td></td>
    <td>NO APROBADO</td>
    <td><a href="https://yostinch.atlassian.net/browse/IEPF-14?atlOrigin=eyJpIjoiMDY4MGIzZDA1YWViNDgzMzljNTgwODEzNjU1ZGNkMzEiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>




  
