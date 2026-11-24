Actúa como un diseñador UX/UI y desarrollador frontend experto en interfaces para aplicaciones con inteligencia artificial (IA). 
Necesito que me ayudes a construir una **maqueta navegable con HTML y CSS** (sin conectar ningún modelo de IA real todavía, ya que primero vamos a validar la experiencia y luego integramos) para un **Asistente con IA** que cumpla con el recorrido completo de interacción y buenas prácticas de UX para LLMs.

### Contexto y principio de diseño
Un LLM puede alucinar, cambiar de respuesta o no saber algo. La interfaz no debe ocultarlo: debe ayudar a entender, verificar y corregir. Diseñar una app con IA también es diseñar sus errores y sus límites con transparencia.

### Requisitos obligatorios de la interfaz y el flujo
1. **Aviso de límites visible en la vista**:
   - Un aviso claro e integrado en la interfaz que indique que es una IA y que puede fallar o cometer errores (por ejemplo, invitando a verificar información importante).
2. **Recorrido completo de una pregunta (estados navegables)**:
   - **Estado Vacío / Consulta**: Un campo de consulta claro, con un ejemplo de pregunta listo para probar o inspirar (ej.: *«¿Cuándo es la sesión de IA?»*), y estado inicial vacío bien explicado.
   - **Estado Cargando / Espera**: Un indicador visual claro de *«Pensando…»* para que el usuario sepa que el sistema está procesando y no crea que se colgó.
   - **Estado Respuesta**: Una respuesta corta, legible y con estructura/formato consistente, acompañada de su **Fuente** (el documento que la respalda, con su enlace).
   - **Estado Error / «No sé»**: Un mensaje honesto y claro (evitando errores técnicos crípticos como un "Error 500" sin contexto) y **opciones de salida**:
     - Reintentar / reformular la pregunta.
     - Escalar o **hablar con una persona** (canal o acción visible de contacto humano).

### Buenas prácticas, casos reales y comparación
- Aplica buenas prácticas de UX en IA: jerarquía visual clara, estados diferenciados y navegables, mensajes honestos, accesibilidad y retroalimentación constante.
- Incluye o ten en cuenta referencias de **casos reales de automatización de empresas con IA** (cómo manejan fuentes, fallos o handoff a humano) para fundamentar las decisiones de diseño.
- Al final, entrégame también:
  1. Un **review breve con evidencia** de lo construido (qué resuelve cada estado y cómo se valida la experiencia).
  2. Una **comparación breve con alguien** (por ejemplo, comparando este enfoque de diseño transparente con errores claros y salida a humano frente a un chatbot tradicional opaco o con errores genéricos, o comparando criterios con un compañero de equipo/revisión).

### Entregable esperado
- Código limpio y modular en **HTML y CSS** (con un JS ligero opcional solo para poder cambiar/navegar entre los estados *Vacío*, *Cargando*, *Respuesta* y *Error/No sé* y probar el flujo).
- Explicación breve de cada estado, el *review* con evidencia y la comparación solicitada.