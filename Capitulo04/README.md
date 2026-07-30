# Flujos de datos con PowerPlatform

## Metadatos

| Campo            | Valor                                                                 |
|------------------|-----------------------------------------------------------------------|
| **Duración**     | 45 minutos                                                            |
| **Complejidad**  | Media                                                                  |
| **Nivel Bloom**  | Aplicar (Apply)                                                       |
| **Módulo**       | Capítulo 4 — Flujos y gobierno en Power Platform                     |
| **Versión**      | 1.0                                                                   |

## Pasos del laboratorio

### Paso 1 — Flujo de Nube con Copilot

En este artículo, creará un flujo de nube, lo probará y luego lo ejecutará. El flujo de nube completado envía un boletín mensual a una dirección de correo electrónico. Para brindarle la experiencia completa, envíe el correo electrónico a su propia dirección para que pueda recibir los resultados del flujo de nube en su bandeja de entrada.

1. Inicie sesión en Power Automate.

2. En el panel de navegación de la izquierda, asegúrese de que Inicio está seleccionado.

3. En el campo Crear la automatización con Copilot, describa qué tipo de flujo desea crear. Utiliza un lenguaje natural y sé lo más específico posible.

4. Copie la solicitud siguiente y péguelo en el campo Copilot:

Solicitud de Copilot
```powershell
Crea un flujo que se ejecute el primer día de cada mes a partir de junio de 2025 a las 12:00 a. m. (hora del Pacífico).

Envíalo a contoso@gmail.com con el asunto "Boletín de Contoso Cadence".

El cuerpo del correo electrónico debe ser:

"¡Bienvenido al boletín mensual de Contoso Cadence! En este correo encontrarás fechas importantes para sesiones de capacitación y charlas. También mostraremos demostraciones y responderemos las preguntas frecuentes del mes."
```

Su solicitud indica Copilot cómo configurar la periodicidad del correo electrónico, quién es el destinatario y el contenido del asunto y el cuerpo del correo electrónico: toda la información que necesita para crear un flujo de nube que funcione.

Una vez que pegue el mensaje, reemplace la dirección de correo electrónico contoso@gmail.com con su propia dirección de correo electrónico.

Si estuvieras haciendo esto en un escenario de la vida real, ingresarías el correo electrónico de la persona a la que deseas enviar el boletín. En este tutorial, use su propio correo electrónico para poder ver los resultados del flujo.

 5. Seleccione Generar.
    En función de la descripción, Copilot comienza a crear un desencadenador y acciones sugeridos para el flujo. Un desencadenador es un evento que inicia un flujo de nube. Las Acciones son los eventos que quiere que haga el flujo después de tener lugar el evento desencadenador.

En este ejemplo, el desencadenador es Periodicidad y la acción es Enviar un correo electrónico.

 6. Seleccione Mantener y continuar.
 7. <img width="1017" height="551" alt="image" src="https://github.com/user-attachments/assets/f9584e7e-bfb8-435a-9452-09fba9721282" />


