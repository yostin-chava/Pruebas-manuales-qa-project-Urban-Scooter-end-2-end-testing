# Tabla lista de comprobación y resultados de las pruebas: prueba de las ventanas "Método de pago" y "Agregar tarjeta"

<table>
  <tr>
    <th>Solicitud</th>
    <th>Descripción de la supervisión</th>
    <th>Estado</th>
    <th>Enlace al informe de errores</th>
    <th>Comentario</th>
  </tr>
  
  <!-- ----- -->
  <!-- Login -->
  <!-- ----- -->
  
  <!-- Numero 1 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con 2 caracteres latinos en el campo login: "ab"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "login".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras latinas con una longitud de 2 caracteres en el login y enviar una solicitud con nombre de usuario y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 201 Created</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "ok": true<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>APROBADO</td>
  </tr>
  <!-- Numero 2 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con 10 caracteres latinos en el campo login: "abcdefghij"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "login".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras latinas con una longitud de 10 caracteres en el login y enviar una solicitud con nombre de usuario y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 201 Created</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "ok": true<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>APROBADO</td>
  </tr>
  <!-- Numero 3 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con 3 caracteres latinos en el campo login: "abc"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "login".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras latinas con una longitud de 3 caracteres en el login y enviar una solicitud con nombre de usuario y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 201 Created</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "ok": true<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>APROBADO</td>
  </tr>
  <!-- Numero 4 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con 9 caracteres latinos en el campo login: "abcdefghi"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "login".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras latinas con una longitud de 9 caracteres en el login y enviar una solicitud con nombre de usuario y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 201 Created</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "ok": true<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>APROBADO</td>
  </tr>
  <!-- Numero 5 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con el espacio vacio en el campo login: ""<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "login".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir un espacio vacío en el login y enviar una solicitud con nombre de usuario y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>APROBADO</td>
  </tr>
  <!-- Numero 6 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con 1 caracter latinos en el campo login: "a"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "login".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras latinas con una longitud de 1 carácter en el login y enviar una solicitud con nombre de usuario y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>NO APROBADO</td>
    <td rowspan="3"><a href="https://yostinch.atlassian.net/browse/IEPF-15?atlOrigin=eyJpIjoiZjBhNzg5ODEyNjZiNGJkZTk4MjUxZDYzZjZiNWFiOWYiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>NO APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>NO APROBADO</td>
  </tr>
  <!-- Numero 7 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con 11 caracteres latino en el campo login: "abcdefghijk"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "login".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras latinas con una longitud de 11 caracteres en el login y enviar una solicitud con nombre de usuario y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>NO APROBADO</td>
    <td rowspan="3"><a href="https://yostinch.atlassian.net/browse/IEPF-16?atlOrigin=eyJpIjoiZWRlY2YwZDdlNGRkNDI0OWFjYmI2NDJjYmU4ZWVmYzciLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>NO APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>NO APROBADO</td>
  </tr>
  <!-- Numero 8 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con 12 caracteres latinos en el campo login: "abcdefghijkl"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "login".</td>
    <td rowspan="5">La prueba fue omitida debido a que no se superó el límite de 11 caracteres.</td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras latinas con una longitud de 12 caracteres en el login y enviar una solicitud con nombre de usuario y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>OMITIDA</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>OMITIDA</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>OMITIDA</td>
  </tr>
  <!-- Numero 9 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con numeros en el campo login: "1234"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "login".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir números en el login y enviar una solicitud con nombre de usuario y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>NO APROBADO</td>
    <td rowspan="3"><a href="https://yostinch.atlassian.net/browse/IEPF-17?atlOrigin=eyJpIjoiODJmMmEwNTY1N2EwNDVkZjk4ODQwMzkzZjIxM2QzMWIiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>NO APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>NO APROBADO</td>
  </tr>
  <!-- Numero 10 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con caracteres chinos en el campo login: "你好"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "login".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras chinas en el login y enviar una solicitud con nombre de usuario y contraseña valida.		</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>NO APROBADO</td>
    <td rowspan="3"><a href="https://yostinch.atlassian.net/browse/IEPF-18?atlOrigin=eyJpIjoiN2ZhZWUxNjk5MjFmNGI5OTgzZDE0YWRlZGZhN2E4MzciLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>NO APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>NO APROBADO</td>
  </tr>
  <!-- Numero 11 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con caracteres especiales en el campo login: "@#*-"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "login".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir caracteres especiales en el login y enviar una solicitud con nombre de usuario y contraseña valida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>NO APROBADO</td>
    <td rowspan="3"><a href="https://yostinch.atlassian.net/browse/IEPF-19?atlOrigin=eyJpIjoiMDY1ZTFiOTgwNWZmNDQ1OGFiOGU5OWE5NzdlZThjYTYiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>NO APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>NO APROBADO</td>
  </tr>
  <!-- Numero 12 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con un loginUser ya registrado.<br>endpoint: POST /api/v1/courierPOST</td>
    <td colspan="3">Probar la entrada de datos en el campo "login".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir un loginUser ya registrado en el login y enviar una solicitud con nombre de usuario y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 409 Сonflict</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "Este inicio de sesión no está disponible"<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>APROBADO</td>
  </tr>

  <!-- --------- -->
  <!-- firstName -->
  <!-- --------- -->
  <tr>
    <td colspan="5"></td>
  </tr>
  
  <!-- Numero 1 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con 2 caracteres latinos en el campo firstName: "ab"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "firstName".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras latinas con una longitud de 2 caracteres en el firstName y enviar una solicitud con login y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 201 Created</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "ok": true<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>APROBADO</td>
  </tr>
  <!-- Numero 2 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con 10 caracteres latinos en el campo firstName: "abcdefghij"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "firstName".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras latinas con una longitud de 10 caracteres en el firstName y enviar una solicitud con login y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 201 Created</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "ok": true<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>APROBADO</td>
  </tr>
  <!-- Numero 3 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con 3 caracteres latinos en el campo firstName: "abc"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "firstName".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras latinas con una longitud de 3 caracteres en el firstName y enviar una solicitud con login y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 201 Created</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "ok": true<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>APROBADO</td>
  </tr>
  <!-- Numero 4 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con 9 caracteres latinos en el campo firstName: "abcdefghi"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "firstName".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras latinas con una longitud de 9 caracteres en el firstName y enviar una solicitud con login y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 201 Created</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "ok": true<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>APROBADO</td>
  </tr>
  <!-- Numero 5 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con el espacio vacio en el campo firstName: ""<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "firstName".</td>
    <td rowspan="5">Zona gris: Según los requisitos, no es necesario ingresar el nombre del repartidor; sin embargo, en el estado del pedido aparece el nombre del repartidor.</td>
  </tr>
  <tr>
    <td colspan="3">Introducir un espacio vacío en el firstName y enviar una solicitud con login y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>APROBADO</td>
  </tr>
  <!-- Numero 6 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con 1 caracter latinos en el campo firstName: "a"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "firstName".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras latinas con una longitud de 1 caracteres en el firstName y enviar una solicitud con login y contraseña valida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>NO APROBADO</td>
    <td rowspan="3"><a href="https://yostinch.atlassian.net/browse/IEPF-20?atlOrigin=eyJpIjoiZjQzNjMyOGY1ZTg2NGNmYmFiMTlhNzE1MzZlNDU0MjkiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>NO APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>NO APROBADO</td>
  </tr>
  <!-- Numero 7 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con 11 caracteres latino en el campo firstName: "abcdefghijk"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "firstName".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras latinas con una longitud de 11 caracteres en el firstName y enviar una solicitud con login y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>NO APROBADO</td>
    <td rowspan="3"><a href="https://yostinch.atlassian.net/browse/IEPF-21?atlOrigin=eyJpIjoiOTM3YjNiMTRhY2IxNDI1Yzk0NTk2YmEzMDRjNTM0NmUiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>NO APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>NO APROBADO</td>
  </tr>
  <!-- Numero 8 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con 12 caracteres latinos en el campo firstName: "abcdefghijkl"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "firstName".</td>
    <td rowspan="5">La prueba fue omitida debido a que no se superó el límite de 11 caracteres.</td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras latinas con una longitud de 12 caracteres en el firstName y enviar una solicitud con login y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>OMITIDA</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>OMITIDA</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>OMITIDA</td>
  </tr>
  <!-- Numero 9 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con numeros en el campo firstName: "1234"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "firstName".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir números en el firstName y enviar una solicitud con login y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>NO APROBADO</td>
    <td rowspan="3"><a href="https://yostinch.atlassian.net/browse/IEPF-22?atlOrigin=eyJpIjoiNjdlZGVjNTJmNDUxNGI3ZGIzODZmYzE2OTMxOTNhNGUiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>NO APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>NO APROBADO</td>
  </tr>
  <!-- Numero 10 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con caracteres chinos en el campo firstName: "你好"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "firstName".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras chinas en el firstName y enviar una solicitud con login y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>NO APROBADO</td>
    <td rowspan="3"><a href="https://yostinch.atlassian.net/browse/IEPF-23?atlOrigin=eyJpIjoiZGQ2MWYwZTJmNjlkNDA2N2I4MDc4ZWQ3YzdmNTg3YmMiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>NO APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>NO APROBADO</td>
  </tr>
  <!-- Numero 11 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con caracteres especiales en el campo firstName: "@#*-"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "firstName".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir caracteres especiales en el firstName y enviar una solicitud con login y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>NO APROBADO</td>
    <td rowspan="3"><a href="https://yostinch.atlassian.net/browse/IEPF-24?atlOrigin=eyJpIjoiNWU3NTc2MGE1MDFhNGFkNjgwOGZhMzkxNzAzOGZiYjgiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>NO APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>NO APROBADO</td>
  </tr>
  <!-- Numero 12 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con un firstName ya registrado.<br>endpoint: POST /api/v1/courierPOST</td>
    <td colspan="3">Probar la entrada de datos en el campo "firstName".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir un nombre ya registrado en el firstName y enviar una solicitud con login y contraseña válida.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 201 Created</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "ok": true<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>APROBADO</td>
  </tr>
  
  <!-- -------- -->
  <!-- password -->
  <!-- -------- -->
  <tr>
    <td colspan="5"></td>
  </tr>
  
  <!-- Numero 1 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con 4 numeros enteros en el campo password: "1234"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "password".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir 4 números enteros en el campo password y enviar una solicitud con un login y firstName válidos.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 201 Created</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "ok": true<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>APROBADO</td>
  </tr>
  <!-- Numero 2 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con 3 numeros enteros en el campo password: "123"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "password".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir 3 números enteros en el campo password y enviar una solicitud con un login y firstName válidos.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>NO APROBADO</td>
    <td rowspan="3"><a href="https://yostinch.atlassian.net/browse/IEPF-25?atlOrigin=eyJpIjoiODU1YWNiMTJlZmE4NGZlMTlhZmY0MWUzMTU3N2U2ZWEiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>NO APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>NO APROBADO</td>
  </tr>
  <!-- Numero 3 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con 5 numeros enteros en el campo password: "12345"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "password".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir 5 números enteros en el campo password y enviar una solicitud con un login y firstName válidos.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>NO APROBADO</td>
    <td rowspan="3"><a href="https://yostinch.atlassian.net/browse/IEPF-26?atlOrigin=eyJpIjoiNzgzYmE4Y2ViYzUxNGJmNThkNjE5NzU3ZGJkMjlhMjIiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>NO APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>NO APROBADO</td>
  </tr>
  <!-- Numero 4 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con caracteres latinos en el campo password: "Hola"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "password".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras latinas en el campo password y enviar una solicitud con un login y firstName válidos.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>NO APROBADO</td>
    <td rowspan="3"><a href="https://yostinch.atlassian.net/browse/IEPF-27?atlOrigin=eyJpIjoiYzRiODE0MjUzNGQwNGU4YThkZDMxMDU0OTJlNDAyNDAiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>NO APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>NO APROBADO</td>
  </tr>
  <!-- Numero 5 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con caracteres chinos en el campo password: "你好"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "password".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir letras chinas en el campo password y enviar una solicitud con un login y firstName válidos.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>NO APROBADO</td>
    <td rowspan="3"><a href="https://yostinch.atlassian.net/browse/IEPF-28?atlOrigin=eyJpIjoiOTc2MDE3NTFlNTliNGI3NmIwOTMzN2ZmNzRmOTNhYjIiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>NO APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>NO APROBADO</td>
  </tr>
  <!-- Numero 6 -->
  <tr>
    <td rowspan="5">Crear un repartidor o repartidora con caracteres especiales en el campo password: "@#*-"<br>endpoint: POST /api/v1/courier</td>
    <td colspan="3">Probar la entrada de datos en el campo "password".</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir caracteres especiales en el campo password y enviar una solicitud con un login y firstName válidos.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>NO APROBADO</td>
    <td rowspan="3"><a href="https://yostinch.atlassian.net/browse/IEPF-29?atlOrigin=eyJpIjoiZWJlNTRhNWE2MjNlNGRmMjg1YWY1YTdiZjljZmY5ZjAiLCJwIjoiaiJ9" target="_blank">Link a Jira</a></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay suficientes datos para crear una cuenta"<br>
     }<br></td>
    <td>NO APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un mensajero en la base de datos, en la tabla "Repartidores".</td>
    <td>NO APROBADO</td>
  </tr>

  <!-- -------------- -->
  <!-- Iniciar sesion -->
  <!-- -------------- -->
  <tr>
    <td colspan="5"></td>
  </tr>
  
  <!-- Numero 1 -->
  <tr>
    <td rowspan="5">Iniciar sesion con un repartidor o repartidora valido.<br>endpoint: POST /api/v1/courier/login</td>
    <td colspan="3">Probar el inicio de sesión.</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir un login y password de un mensajero válidos.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 200 OK</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           id: 12345<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que se creó un registro en la base de datos, en la tabla "Repartidores".</td>
    <td>APROBADO</td>
  </tr>
  <!-- Numero 2 -->
  <tr>
    <td rowspan="5">Iniciar sesion con un repartidor o repartidora sin login ni contraseña.<br>endpoint: POST /api/v1/courier/login</td>
    <td colspan="3">Probar el inicio de sesión.</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">No introducir login ni password al iniciar sesión.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 400 Bad Request</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "No hay datos suficientes para iniciar sesión"<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un registro en la base de datos, en la tabla "Repartidores".</td>
    <td>APROBADO</td>
  </tr>
  <!-- Numero 3 -->
  <tr>
    <td rowspan="5">Iniciar sesion con un repartidor o repartidora con login y contraseña inexistente.<br>endpoint: POST /api/v1/courier/login</td>
    <td colspan="3">Probar el inicio de sesión.</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir login y contraseña inexistente.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 404 Not found</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
           "message": "Account not found"<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que no se creó un registro en la base de datos, en la tabla "Repartidores".</td>
    <td>APROBADO</td>
  </tr>

  <!-- ------------------- -->
  <!-- Eliminar repartidor -->
  <!-- ------------------- -->
  <tr>
    <td colspan="5"></td>
  </tr>
  
  <!-- Numero 1 -->
  <tr>
    <td rowspan="5">Eliminar un repartidor o repartidora con id de mensajero existente.<br>endpoint: DELETE /api/v1/courier/:id</td>
    <td colspan="3">Probar eliminar mensajero.</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">Introducir el id de un mensajero registrado.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 200 OK</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
          "ok": true<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que al eliminar el mensajero, los pedidos vinculados en la tabla "Orders (Pedidos)" deben borrarse.</td>
    <td>APROBADO</td>
  </tr>
  <!-- Numero 2 -->
  <tr>
    <td rowspan="5">Eliminar un repartidor o repartidora con id inexistente.<br>endpoint: DELETE /api/v1/courier/:id</td>
    <td colspan="3">Probar eliminar mensajero.</td>
    <td rowspan="5"></td>
  </tr>
  <tr>
    <td colspan="3">No introducir el id en la solicitud.</td>
  </tr>
  <tr>
    <td>Código respuesta de la API: 200 OK</td>
    <td>APROBADO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>Cuerpo de la respuesta:<br>
     {<br>
          "ok": true<br>
     }<br></td>
    <td>APROBADO</td>
  </tr>
  <tr>
    <td>Probar que al eliminar el mensajero, los pedidos vinculados en la tabla "Orders (Pedidos)" deben borrarse.</td>
    <td>APROBADO</td>
  </tr>

  
  
  
 
 
  

     

      
</table>
