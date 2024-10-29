# README - Manejo del Modal e Interacción de Chat

Este código en JavaScript proporciona funcionalidad para manejar un modal emergente e implementar una interfaz de chat simulada en la que los usuarios pueden ingresar y recibir respuestas predefinidas en función de sus entradas. Utiliza la API DOM para gestionar la visibilidad del modal, capturar la entrada del usuario y simular respuestas en el chat, e incluye animaciones y alertas básicas.

---

## Tabla de Contenidos

1. [Configuración](#configuración)
2. [Manejo del Modal](#manejo-del-modal)
3. [Simulación de Chat](#simulación-de-chat)
   - [Manejo de Entradas del Usuario](#manejo-de-entradas-del-usuario)
   - [Opciones de Chat](#opciones-de-chat)
   - [Alertas](#alertas)
4. [Instrucciones de Uso](#instrucciones-de-uso)
5. [Descripción del Código](#descripción-del-código)

---

### Configuración

Asegúrate de tener los siguientes elementos en tu HTML para que el código JavaScript funcione correctamente:

- Un botón con el ID `mostrar-modal-boot` para abrir el modal.
- Un contenedor de modal con el ID `myModal-boot`.
- Un botón de cierre dentro del modal con la clase `close-modal-boot`.
- Un campo de entrada con el ID `respuesta-user` para las respuestas del usuario.
- Un contenedor con el ID `chat-body` para mostrar los mensajes del chat.

### Manejo del Modal

El código gestiona la visualización de una ventana modal donde:

- Al hacer clic en el botón con el ID `mostrar-modal-boot` se abre el modal.
- Al hacer clic en el botón de cierre (con la clase `close-modal-boot`) se oculta el modal.

### Simulación de Chat

La simulación de chat permite al usuario interactuar en una experiencia de chat simulada donde puede:

1. Ingresar su nombre y número de teléfono.
2. Elegir entre opciones predefinidas para hacer preguntas o programar una llamada de retorno.

#### Manejo de Entradas del Usuario

- Las entradas del usuario se capturan a través del campo de entrada con el ID `respuesta-user`.
- El botón `enviarSms` envía la entrada a la interfaz de chat.

#### Opciones de Chat

Dependiendo de las elecciones del usuario, se le presentan:

- Consultas frecuentes sobre compras, envíos y métodos de pago.
- Opciones para programar una llamada en horarios específicos.

#### Alertas

Se utiliza SweetAlert2 para mostrar alertas personalizadas con títulos, textos e íconos que mejoran la retroalimentación del usuario. Por ejemplo, una alerta confirma una llamada programada basada en la entrada del usuario.

### Instrucciones de Uso

1. **Abrir el Modal:** Haz clic en el botón asociado al ID `mostrar-modal-boot`.
2. **Interacción con el Chat:** Ingresa los datos solicitados por la interfaz de chat. Según la opción ingresada, el usuario recibirá respuestas predefinidas y podrá programar una llamada.
3. **Cerrar el Modal:** Haz clic en el botón de cierre dentro del modal.

### Descripción del Código

El código está organizado de la siguiente manera:

- **Visibilidad del Modal:** Alterna los estilos de visualización para mostrar y ocultar el modal.
- **Captura de Datos del Usuario:** Recoge el nombre y número de teléfono.
- **Opciones de Chat Predefinidas:** Responde a las opciones seleccionadas por el usuario con la información relevante o programación de llamadas.
- **Programación de Llamadas:** Permite al usuario programar una llamada en rangos de tiempo específicos.
- **Alertas:** SweetAlert2 muestra mensajes de confirmación y error.

Este código sirve como sistema básico de interacción para el manejo de un modal y simulación de chat, que se puede personalizar o ampliar según los requisitos específicos de interacción con el usuario.

---

**Nota:** Esta implementación depende de SweetAlert2 para la gestión de alertas. Asegúrate de cargar SweetAlert2 en tu proyecto.
