# Tabla casos de prueba y pruebas: la lógica de las funciones de reserva

<div style="overflow-x:auto;">
  <table>

  <tr>
    <th>ID</th>
    <th>Título</th>
    <th>Condición previa</th>
    <th>Pasos</th>
    <th>Descripción de los pasos</th>
    <th>Resultado esperado</th>
    <th>Version</th>
    <th>Estado</th>
    <th>Enlace a los informes de errores</th>
    <th>Comentarios</th>
  </tr>
  <!-- Caso 1 -->
  <tr>
    <td rowspan="2">1</td>
    <td rowspan="2">Verificar que aparezca una notificación cuando falten 2 horas para finalizar el pedido. Hora 10pm.</td>
    <td rowspan="2"><pre>1. El usuario o usuaria ha realizado un pedido.<br>2. Abre la aplicación móvil.<br>3. Inicia sesión como un repartidor o repartidora que no tiene pedidos.</pre></td>
    <td>1</td>
    <td>Aceptar el pedido</td>
    <td rowspan="2">Aparece una ventanas emergente cuando faltan 2 horas para que se termine el tiempo de entrega del pedido.</td>
    <td rowspan="2"><pre>Emulador de Android Studio,<br>Dispositivo movil: Pixel 9,<br>SO: Android 16</pre></td>
    <td rowspan="2">OMITIDO</td>
    <td rowspan="2"></td>
    <td rowspan="21">La prueba para verificar el funcionamiento y diseño de la notificación que debe aparecer dos horas antes de que finalice el pedido fue omitida, ya que no es posible ejecutarla debido a que el servidor está adelantado con respecto a la hora local. Además, no se cuentan con los permisos necesarios para modificar la hora del sistema, ni es posible contactar al área de desarrollo para coordinar una forma de simular el escenario requerido.</td>
  </tr>
  <tr>
    <td>2</td>
    <td>Dar clic en "Si" aceptar el pedido</td>
  </tr>
  <!-- Caso 2 -->
  <tr>
    <td rowspan="2">2</td>
    <td rowspan="2">Verificar que aparezca una notificación cuando falten 2 horas para finalizar el pedido. Hora 9:59pm.</td>
    <td rowspan="2"><pre>1. El usuario o usuaria ha realizado un pedido.<br>2. Abre la aplicación móvil.<br>3. Inicia sesión como un repartidor o repartidora que no tiene pedidos.</pre></td>
    <td>1</td>
    <td>Aceptar el pedido</td>
    <td rowspan="2">La ventana emergente no aparece.</td>
    <td rowspan="2"><pre>Emulador de Android Studio,<br>Dispositivo movil: Pixel 9,<br>SO: Android 16</pre></td>
    <td rowspan="2">OMITIDO</td>
    <td rowspan="2"></td>
  </tr>
  <tr>
    <td>2</td>
    <td>Dar clic en "Si" aceptar el pedido</td>
  </tr>
  <!-- Caso 3 -->
  <tr>
    <td rowspan="2">3</td>
    <td rowspan="2">Verificar que aparezca una notificación cuando falten 2 horas para finalizar el pedido. Hora 10:01pm.</td>
    <td rowspan="2"><pre>1. El usuario o usuaria ha realizado un pedido.<br>2. Abre la aplicación móvil.<br>3. Inicia sesión como un repartidor o repartidora que no tiene pedidos.</pre></td>
    <td>1</td>
    <td>Aceptar el pedido</td>
    <td rowspan="2">La ventana emergente no aparece.</td>
    <td rowspan="2"><pre>Emulador de Android Studio,<br>Dispositivo movil: Pixel 9,<br>SO: Android 16</pre></td>
    <td rowspan="2">OMITIDO</td>
    <td rowspan="2"></td>
  </tr>
  <tr>
    <td>2</td>
    <td>Dar clic en "Si" aceptar el pedido</td>
  </tr>
  <!-- Caso 4 -->
  <tr>
    <td rowspan="2">4</td>
    <td rowspan="2">Verificar que al tocar la notificación  "2 horas para finalizar el pedido", se navega a la pestaña "Mis pedidos" en la app móvil.</td>
    <td rowspan="2"><pre>1. El usuario o usuaria ha realizado un pedido.<br>2. Abre la aplicación móvil.<br>3. Inicia sesión como un repartidor o repartidora que no tiene pedidos.</pre></td>
    <td>1</td>
    <td>Aceptar el pedido</td>
    <td rowspan="2">Al tocar la notificacion se abre la pestaña "Mis pedidos".</td>
    <td rowspan="2"><pre>Emulador de Android Studio,<br>Dispositivo movil: Pixel 9,<br>SO: Android 16</pre></td>
    <td rowspan="2">OMITIDO</td>
    <td rowspan="2"></td>
  </tr>
  <tr>
    <td>2</td>
    <td>Dar clic en "Si" aceptar el pedido</td>
  </tr>
  <!-- Caso 5 -->
  <tr>
    <td rowspan="2">5</td>
    <td rowspan="2">Verificar que la notificación "2 horas para finalizar el pedido" muestre el ícono de Urban Scooter según el diseño UI en Figma.</td>
    <td rowspan="2"><pre>1. El usuario o usuaria ha realizado un pedido.<br>2. Abre la aplicación móvil.<br>3. Inicia sesión como un repartidor o repartidora que no tiene pedidos.</pre></td>
    <td>1</td>
    <td>Aceptar el pedido</td>
    <td rowspan="2">La notificacion muestra el icono segun su diseño en figma.</td>
    <td rowspan="2"><pre>Emulador de Android Studio,<br>Dispositivo movil: Pixel 9,<br>SO: Android 16</pre></td>
    <td rowspan="2">OMITIDO</td>
    <td rowspan="2"></td>
  </tr>
  <tr>
    <td>2</td>
    <td>Dar clic en "Si" aceptar el pedido</td>
  </tr>
  <!-- Caso 6 -->
  <tr>
    <td rowspan="2">6</td>
    <td rowspan="2">Verificar que la notificación tenga el título: "Urban Scooter".</td>
    <td rowspan="2"><pre>1. El usuario o usuaria ha realizado un pedido.<br>2. Abre la aplicación móvil.<br>3. Inicia sesión como un repartidor o repartidora que no tiene pedidos.</pre></td>
    <td>1</td>
    <td>Aceptar el pedido</td>
    <td rowspan="2">La notificacion tiene el titulo "Urban Scooter".</td>
    <td rowspan="2"><pre>Emulador de Android Studio,<br>Dispositivo movil: Pixel 9,<br>SO: Android 16</pre></td>
    <td rowspan="2">OMITIDO</td>
    <td rowspan="2"></td>
  </tr>
  <tr>
    <td>2</td>
    <td>Dar clic en "Si" aceptar el pedido</td>
  </tr>
  <!-- Caso 7 -->
  <tr>
    <td rowspan="2">7</td>
    <td rowspan="2">Verificar que la notificación muestre el mensaje: "2 horas hasta el final del pedido. Se debe completar el pedido 'State St 1214'. Si no llegas a tiempo, contacta a soporte: 0101".</td>
    <td rowspan="2"><pre>1. El usuario o usuaria ha realizado un pedido.<br>2. Abre la aplicación móvil.<br>3. Inicia sesión como un repartidor o repartidora que no tiene pedidos.</pre></td>
    <td>1</td>
    <td>Aceptar el pedido</td>
    <td rowspan="2">La notificaicon contiene el mensaje "2 horas hasta el final del pedido. Se debe completar el pedido 'State St 1214'. Si no llegas a tiempo, contacta a soporte: 0101".</td>
    <td rowspan="2"><pre>Emulador de Android Studio,<br>Dispositivo movil: Pixel 9,<br>SO: Android 16</pre></td>
    <td rowspan="2">OMITIDO</td>
    <td rowspan="2"></td>
  </tr>
  <tr>
    <td>2</td>
    <td>Dar clic en "Si" aceptar el pedido</td>
  </tr>
  <!-- Caso 8 -->
  <tr>
    <td rowspan="3">8</td>
    <td rowspan="3">Verificar que aparezca una notificación cuando falten 2 horas para finalizar el pedido cuando el celular este bloqueado.</td>
    <td rowspan="3"><pre>1. El usuario o usuaria ha realizado un pedido.<br>2. Abre la aplicación móvil.<br>3. Inicia sesión como un repartidor o repartidora que no tiene pedidos.</pre></td>
    <td>1</td>
    <td>Aceptar el pedido</td>
    <td rowspan="3">Aparece una ventanas emergente cuando faltan 2 horas para que se termine el tiempo de entrega del pedido.</td>
    <td rowspan="3"><pre>Emulador de Android Studio,<br>Dispositivo movil: Pixel 9,<br>SO: Android 16</pre></td>
    <td rowspan="3">OMITIDO</td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>2</td>
    <td>Dar clic en "Si" aceptar el pedido</td>
  </tr>
  <tr>
    <td>3</td>
    <td>Cerrar la aplicación</td>
  </tr>
  <!-- Caso 9 -->
  <tr>
    <td rowspan="4">9</td>
    <td rowspan="4">Verificar que aparezca una notificación cuando falten 2 horas para finalizar el pedido cuando no se esta usando la aplicación.</td>
    <td rowspan="4"><pre>1. El usuario o usuaria ha realizado un pedido.<br>2. Abre la aplicación móvil.<br>3. Inicia sesión como un repartidor o repartidora que no tiene pedidos.</pre></td>
    <td>1</td>
    <td>Aceptar el pedido</td>
    <td rowspan="4">Aparece una ventanas emergente cuando faltan 2 horas para que se termine el tiempo de entrega del pedido.</td>
    <td rowspan="4"><pre>Emulador de Android Studio,<br>Dispositivo movil: Pixel 9,<br>SO: Android 16</pre></td>
    <td rowspan="4">OMITIDO</td>
    <td rowspan="4"></td>
  </tr>
  <tr>
    <td>2</td>
    <td>Dar clic en "Si" aceptar el pedido</td>
  </tr>
  <tr>
    <td>3</td>
    <td>Cerrar la aplicación</td>
  </tr>
  <tr>
    <td>4</td>
    <td>Bloquear el celular</td>
  </tr>
  <!-- Caso 10 -->
  <tr>
    <td rowspan="2">10</td>
    <td rowspan="2">Verificar que al no haber acceso a internet y al interactuar con la aplicación, aparezca una ventana emergente.</td>
    <td rowspan="2"><pre>1. El usuario o usuaria ha realizado un pedido.<br>2. Abre la aplicación móvil.<br>3. Inicia sesión como un repartidor o repartidora que no tiene pedidos.</pre></td>
    <td>1</td>
    <td>Desconectar el internet</td>
    <td rowspan="2">Aparece una ventanas emergente cuando no hay acceso a internet.</td>
    <td rowspan="2"><pre>Emulador de Android Studio,<br>Dispositivo movil: Pixel 9,<br>SO: Android 16</pre></td>
    <td rowspan="2">APROBADO</td>
    <td rowspan="2"></td>
    <td rowspan="2"></td>
  </tr>
  <tr>
    <td>2</td>
    <td>Interactuar con la aplicación</td>
  </tr>
  <!-- Caso 11 -->
  <tr>
    <td rowspan="2">11</td>
    <td rowspan="2">Verificar que la ventana emergente contenga el texto "Sin acceso a Internet".</td>
    <td rowspan="2"><pre>1. El usuario o usuaria ha realizado un pedido.<br>2. Abre la aplicación móvil.<br>3. Inicia sesión como un repartidor o repartidora que no tiene pedidos.</pre></td>
    <td>1</td>
    <td>Desconectar el internet</td>
    <td rowspan="2">La ventana emergente contiene el texto "Sin acceso a Internet".</td>
    <td rowspan="2"><pre>Emulador de Android Studio,<br>Dispositivo movil: Pixel 9,<br>SO: Android 16</pre></td>
    <td rowspan="2">APROBADO</td>
    <td rowspan="2"></td>
    <td rowspan="2"></td>
  </tr>
  <tr>
    <td>2</td>
    <td>Interactuar con la aplicación</td>
  </tr>
  <!-- Caso 12 -->
  <tr>
    <td rowspan="2">12</td>
    <td rowspan="2">Verificar que la ventana emergente "Sin acceso a internet" muestre debajo el texto: "Comprueba la conexión o espera una notificación de que se ha restablecido".</td>
    <td rowspan="2"><pre>1. El usuario o usuaria ha realizado un pedido.<br>2. Abre la aplicación móvil.<br>3. Inicia sesión como un repartidor o repartidora que no tiene pedidos.</pre></td>
    <td>1</td>
    <td>Desconectar el internet</td>
    <td rowspan="2">La ventana emergente contiene el texto "Comprueba la conexión o espera una notificación de que se ha restablecido".</td>
    <td rowspan="2"><pre>Emulador de Android Studio,<br>Dispositivo movil: Pixel 9,<br>SO: Android 16</pre></td>
    <td rowspan="2">APROBADO</td>
    <td rowspan="2"></td>
    <td rowspan="2"></td>
  </tr>
  <tr>
    <td>2</td>
    <td>Interactuar con la aplicación</td>
  </tr>
  <!-- Caso 13 -->
  <tr>
    <td rowspan="2">13</td>
    <td rowspan="2">Verificar que la ventana emergente "Sin acceso a internet" muestre un boton "Aceptar".</td>
    <td rowspan="2"><pre>1. El usuario o usuaria ha realizado un pedido.<br>2. Abre la aplicación móvil.<br>3. Inicia sesión como un repartidor o repartidora que no tiene pedidos.</pre></td>
    <td>1</td>
    <td>Desconectar el internet</td>
    <td rowspan="2">La ventana emergente contiene el boton con el texto "Aceptar".</td>
    <td rowspan="2"><pre>Emulador de Android Studio,<br>Dispositivo movil: Pixel 9,<br>SO: Android 16</pre></td>
    <td rowspan="2">OMITIDO</td>
    <td rowspan="2"></td>
    <td rowspan="2">La prueba fue omitida debido a una inconsistencia entre los requisitos y el diseño en Figma. Según los requisitos, el botón debería llamarse "Aceptar", pero en el diseño de Figma aparece como "OK".</td>
  </tr>
  <tr>
    <td>2</td>
    <td>Interactuar con la aplicación</td>
  </tr>
  <!-- Caso 14 -->
  <tr>
    <td rowspan="3">14</td>
    <td rowspan="3">Verificar que al tocar el botón "Aceptar", la ventana emergente "Sin acceso a internet" se cierre correctamente.</td>
    <td rowspan="3"><pre>1. El usuario o usuaria ha realizado un pedido.<br>2. Abre la aplicación móvil.<br>3. Inicia sesión como un repartidor o repartidora que no tiene pedidos.</pre></td>
    <td>1</td>
    <td>Desconectar el internet</td>
    <td rowspan="3">La ventana emergente se cierra al dar click en el botón aceptar.</td>
    <td rowspan="3"><pre>Emulador de Android Studio,<br>Dispositivo movil: Pixel 9,<br>SO: Android 16</pre></td>
    <td rowspan="3">APROBADO</td>
    <td rowspan="3"></td>
    <td rowspan="3"></td>
  </tr>
  <tr>
    <td>2</td>
    <td>Interactuar con la aplicación</td>
  </tr>
  <tr>
    <td>3</td>
    <td>Dar clic en el botón aceptar</td>
  </tr>
  <!-- Caso 15 -->
  <tr>
    <td rowspan="4">15</td>
    <td rowspan="4">Verificar que si no hay conexión a Internet, la ventana emergente "Sin acceso a Internet" se muestra nuevamente y el proceso se repite.</td>
    <td rowspan="4"><pre>1. El usuario o usuaria ha realizado un pedido.<br>2. Abre la aplicación móvil.<br>3. Inicia sesión como un repartidor o repartidora que no tiene pedidos.</pre></td>
    <td>1</td>
    <td>Desconectar el internet</td>
    <td rowspan="4">La ventana emergente contiene el texto "Comprueba la conexión o espera una notificación de que se ha restablecido".</td>
    <td rowspan="4"><pre>Emulador de Android Studio,<br>Dispositivo movil: Pixel 9,<br>SO: Android 16</pre></td>
    <td rowspan="4">APROBADO</td>
    <td rowspan="4"></td>
    <td rowspan="4"></td>
  </tr>
  <tr>
    <td>2</td>
    <td>Interactuar con la aplicación</td>
  </tr>
  <tr>
    <td>3</td>
    <td>Dar clic en el botón aceptar</td>
  </tr>
  <tr>
    <td>4</td>
    <td>Volver a interactuar con la aplicación</td>
  </tr>
    
  
