# Pomorun

## Plan de Desarrollo (basado en el arte conceptual)

### 1. Análisis del arte conceptual y requisitos
**Características principales identificadas:**
- Sistema de Pomodoros con temporizador.
- Selección de duración (25, 40, 50 min).
- Seguimiento de objetivos.
- Registro de sesiones y estadísticas.
- Sistema de descansos.
- Opción Premium (sin anuncios, análisis avanzado).
- Autenticación de usuarios.

### 2. Arquitectura técnica
**Stack tecnológico:**
- Lenguaje: Kotlin (Android moderno).
- Arquitectura: MVVM (Model-View-ViewModel).
- Persistencia local: Room Database.
- Autenticación: Firebase Auth.
- Monetización: Google Play Billing para suscripciones.
- Notificaciones: WorkManager para temporizadores en segundo plano.
- UI: Jetpack Compose (moderna y declarativa).

### 3. Estructura de módulos/funcionalidades
**Módulo 1: Autenticación y Onboarding**
- Pantalla de inicio de sesión/registro.
- Onboarding explicando la técnica Pomodoro.
- Sincronización con Firebase.

**Módulo 2: Núcleo Pomodoro**
- Pantalla principal del temporizador:
  - Selector de duración (25/40/50 min).
  - Botón "Correr Pomodoro".
  - Temporizador circular con progreso visual.
  - Controles de pausa/reinicio.
- Sistema de notificaciones:
  - Sonido/vibración al terminar sesión.
  - Notificación persistente durante el Pomodoro.
  - Soporte para modo Do Not Disturb.

**Módulo 3: Seguimiento y Objetivos**
- Pantalla de objetivos diarios:
  - Formulario "¿Qué vas a lograr?".
  - Selección de capítulo/tarea.
- Pantalla de evaluación post-sesión:
  - Opciones: Sí / Más o menos / No.
  - Notas opcionales.
- Historial de sesiones.

**Módulo 4: Descansos y Tips**
- Pantalla de descanso:
  - Temporizador de descanso (ej: 8:00).
  - Tips de estudio motivacionales.
  - Integración con respiraciones guiadas (opcional).
- Sistema de tips aleatorios.

**Módulo 5: Estadísticas y Progreso**
- Dashboard de progreso:
  - Pomodoros hoy/total.
  - Tiempo total estudiado.
  - Racha de días consecutivos.
  - Gráficos de productividad.
  - Análisis semanal/mensual.

**Módulo 6: Monetización (Premium)**
- Pantalla de suscripción:
  - Características Premium vs Free.
  - Integración con Google Play Billing.
  - Gestión de suscripciones.
- Funcionalidades Premium:
  - Sin anuncios.
  - Análisis de productividad avanzado.
  - Temas personalizados.
  - Estadísticas históricas ilimitadas.

**Módulo 7: Configuración y Personalización**
- Ajustes de temporizador.
- Personalización de sonidos.
- Configuración de notificaciones.
- Sincronización en la nube.
- Exportación de datos.

### 4. Plan de desarrollo por sprints (Agile)
**Sprint 1 (2 semanas): MVP básico**
- Configuración del proyecto Android.
- Pantalla de temporizador básico.
- Sistema de Pomodoro funcional.
- Notificaciones locales.

**Sprint 2 (2 semanas): Flujo principal**
- Pantalla de objetivos.
- Evaluación post-sesión.
- Almacenamiento local de sesiones.
- Pantalla de descanso básica.

**Sprint 3 (2 semanas): Seguimiento y UI**
- Dashboard de estadísticas.
- Gráficos básicos.
- UI/UX refinada según arte conceptual.
- Sistema de tips.

**Sprint 4 (2 semanas): Autenticación y nube**
- Integración con Firebase.
- Sincronización de datos.
- Backup/restauración.
- Pantalla de perfil.

**Sprint 5 (2 semanas): Monetización**
- Sistema de anuncios (AdMob).
- Integración de suscripciones Premium.
- Desbloqueo de características Premium.

**Sprint 6 (2 semanas): Pulido y testing**
- Testing (unitarios, instrumentados).
- Optimización de rendimiento.
- Internacionalización (inglés/español).
- Publicación en Play Store.

### 5. Diseño UI/UX
**Paleta de colores (basada en arte conceptual):**
- Principal: Naranja pomodoro (#FF6B35).
- Secundario: Azul profesional (#2D3047).
- Fondo claro: #F8F9FA.
- Texto: #212529.

**Componentes reutilizables:**
- Botones con esquinas redondeadas.
- Cards para estadísticas.
- Temporizador circular animado.
- Selectores de tiempo.
- Modales de evaluación.

### 6. Consideraciones especiales
**Manejo de segundo plano:**
- WorkManager para temporizadores precisos.
- Foreground Service durante Pomodoros activos.
- Manejo adecuado de Doze Mode.

**Accesibilidad:**
- Soporte para TalkBack.
- Contraste adecuado.
- Tamaños de texto escalables.

**Privacidad y términos:**
- Política de privacidad.
- Términos de servicio.
- Cumplimiento GDPR (si aplica).

### 7. Roadmap post-lanzamiento
**Versión 1.1:**
- Widgets de Android.
- Integración con calendario.
- Modos de enfoque adicionales.

**Versión 1.2:**
- Comunidad y retos.
- Logros y gamificación.
- Compartir progreso en redes.

**Versión 2.0:**
- Versión iOS.
- Versión web.
- API pública para desarrolladores.

### 8. Recursos necesarios
**Equipo mínimo:**
- 1 Desarrollador Android.
- 1 Diseñador UI/UX.
- 1 Product Manager (puede ser el mismo desarrollador inicialmente).

**Herramientas:**
- Android Studio.
- Figma/Sketch para diseño.
- Firebase Console.
- Google Play Console.

**Timeline estimado:**
- Desarrollo: 12 semanas (3 meses).
- Testing y lanzamiento: 2 semanas.
- Total: 14 semanas (~3.5 meses).
