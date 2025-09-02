# 🛴 Pruebas Manuales – Urban Scooter (End-to-End Testing)

## 📌 Descripción del proyecto
**Urban Scooter** es una aplicación que permite a las personas usuarias alquilar scooters eléctricos.  
Cuenta con:
- Aplicación web  
- Aplicación móvil  
- API  
- Base de datos **PostgreSQL**  

Este repositorio contiene la documentación de las **pruebas manuales** realizadas a la aplicación.  
Durante el proceso se identificaron y documentaron **errores (bugs)**, así como **comportamientos esperados y no esperados** del sistema.

---

## ✅ Pruebas realizadas
1. **Mapa mental** para la función del formulario de pedido en la aplicación web.  
2. **Lista de comprobación** de la lógica y el diseño de la pantalla **“Estado del pedido”** de la aplicación web.  
3. **Validación de campos** en la pantalla **“Hacer pedido”** de la aplicación web.  
4. **Casos de prueba** para verificar:  
   - Notificación de **“Sin acceso a internet”**.  
   - Notificación que se envía cuando faltan **dos horas** para finalizar el tiempo máximo de entrega del scooter.  
5. **Pruebas de API y base de datos** en los siguientes endpoints:  
   - Crear repartidor/a → validación con **clases de equivalencia** y **valores límite**.  
   - Iniciar sesión con repartidor/a.  
   - Eliminar repartidor/a.  
   - Obtener un pedido mediante su **track**.  
   - Para estos endpoints se aplicaron **clases de equivalencia**, **valores límite** y **pruebas por pares**.  

📌 Todos los errores encontrados fueron registrados en **Jira** para su seguimiento.  

---

## 🛠️ Herramientas utilizadas
- **Navegadores web:** Chrome, Opera  
- **Herramientas de desarrollo:** DevTools (inspección de elementos, monitoreo de red, consola, etc.)  
- **Figma:** verificación de diseño  
- **Postman:** pruebas de API  
- **Android Studio:** simulación de dispositivo Android  
- **Base de datos PostgreSQL:** consultas SQL para verificación de datos  
- **Documentación manual en Markdown**, incluyendo:  
  - Listas de comprobación (checklists)  
  - Casos de prueba  
  - Clases de equivalencia  
  - Valores límite  
  - Diagramas de flujo  
  - Mapas mentales  
- **Jira:** registro y seguimiento de bugs  

---
