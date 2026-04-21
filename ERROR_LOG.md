# ⚠️ Registro de Errores y "Piedras en el Camino"

### Tópico: Gestión de Horarios (Timezones)
* **Error:** Usar el objeto `Date` nativo de JS sin considerar el desfase de la zona horaria del servidor vs el cliente.
* **Solución:** Almacenar todo en **UTC** y usar bibliotecas como `Day.js` o `date-fns-tz` para la visualización local en Maracaibo.

### Tópico: Concurrencia en Reservas
* **Error:** Permitir que dos clientes seleccionen el mismo barbero en el mismo bloque de tiempo por milisegundos de diferencia.
* **Solución:** Implementar **transacciones de base de datos** en Prisma y un bloqueo optimista o validación estricta en el `onSumbit`.

### Tópico: Rendimiento en Móviles
* **Error:** Cargar imágenes de "cortes de pelo" en alta resolución sin optimizar.
* **Solución:** Usar el componente `<Image />` de Next.js para servirlas en formato **WebP** y con lazy loading por defecto.

### Tópico: Autenticación
* **Error:** Persistencia de sesión inestable en WebViews de móviles.
* **Solución:** Configuración correcta de cookies `SameSite` y `Secure`.