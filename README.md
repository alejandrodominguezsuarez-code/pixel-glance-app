# 📱 De Un Vistazo XL — Custom Pixel Widget

Widget personalizado y nativo para la pantalla de inicio de Google Pixel (optimizado para Pixel 6 Pro), diseñado para mostrar de un vistazo los eventos del **Google Calendar** en las próximas **2 horas** con colores dinámicos semafóricos y actualización en tiempo real.

---

## ✨ Características Principales

* **Reloj Dinámico y Tiempo Real:** Utiliza un servicio en segundo plano (`AlarmManager`) para actualizar los minutos restantes de cada evento automáticamente cada minuto, evitando las restricciones de batería de Android.
* **Sistema Semafórico de Colores:** 
  * 🟢 **Verde:** Más de 1 hora restante.
  * 🟠 **Naranja:** Menos de 1 hora restante (≤ 60 min).
  * 🔴 **Rojo:** Inminente o a punto de empezar (≤ 15 min).
* **Detección Automática de Iconos (Flairs):** Reconoce palabras clave en el título de tus eventos para inyectar iconos personalizados:
  * 🦷 *Dentista*
  * ⚕️ *Médico / Consulta*
  * 📅 *Resto de eventos*
* **Multievento Simultáneo:** Lista todos los eventos programados en la ventana de las próximas 2 horas ordenados cronológicamente.
* **Personalización de Fondo al Vuelo:** Menú de configuración accesible tocando el título del widget para elegir entre:
  * Cristal Oscuro (Recomendado para contraste).
  * Totalmente Transparente.
  * Dinámico del Sistema (Material You).
* **Interacciones Directas:**
  * Tocar el **título**: Abre la pantalla de configuración de diseño.
  * Tocar el **cuerpo de los eventos**: Abre la app oficial de Google Calendar.
  * Tocar el **botón 🔄**: Fuerza una lectura instantánea del calendario.

---

## 🛠️ Especificaciones Técnicas

* **Plataforma:** Android (Min SDK 26, Target SDK 34).
* **Lenguaje:** Kotlin / XML Layouts.
* **Automatización:** Compilación nativa mediante GitHub Actions (JDK 17 + Gradle 8.4).
* **Permisos requeridos:** `READ_CALENDAR`, `USE_EXACT_ALARM`.
