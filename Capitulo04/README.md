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

<img width="585" height="292" alt="image" src="https://github.com/user-attachments/assets/4fc4a88a-3163-445e-9160-54a762407d86" />

En función de la descripción, Copilot comienza a crear un desencadenador y acciones sugeridos para el flujo. Un desencadenador es un evento que inicia un flujo de nube. Las Acciones son los eventos que quiere que haga el flujo después de tener lugar el evento desencadenador.

En este ejemplo, el desencadenador es Periodicidad y la acción es Enviar un correo electrónico.

 6. Seleccione Mantener y continuar.
<img width="1017" height="551" alt="image" src="https://github.com/user-attachments/assets/f9584e7e-bfb8-435a-9452-09fba9721282" />

Revise las aplicaciones y los servicios conectados. Una marca de verificación verde indica que la conexión es válida. En este tutorial, la conexión es Office 365 Outlook.

Algunas conexiones le piden que inicie sesión. Si no ha iniciado sesión, seleccione el botón Iniciar sesión y proporcione sus credenciales.

8. Seleccione Crear flujo.

El flujo consta del desencadenador de Periodicidad y la acción Enviar un correo electrónico en función de su solicitud.

<img width="547" height="513" alt="image" src="https://github.com/user-attachments/assets/447eb8b1-5413-479e-b0ee-4dd2407d2bd4" />


9. Guarde su flujo de nube seleccionando el botón Guardar en la barra de comandos superior en la pantalla.

Aparece un mensaje verde debajo de la barra de comandos, lo que indica que el flujo se ha guardado.

<img width="370" height="65" alt="image" src="https://github.com/user-attachments/assets/77c3f9f0-48fa-4f77-a569-9f8254c6a0e0" />

Una vez que cree un flujo, le recomendamos que lo pruebe

##Probar su flujo de nube.

Para asegurarse de que el flujo funciona según lo esperado, debe probarlo.

Asegúrese de haber completado Crear un flujo de nube.


1. En la barra de herramientas, seleccione Probar.

2. En el panel Probar el flujo, seleccione Manualmente y, a continuación, Probar.

3. En el panel Ejecutar flujo, seleccione Ejecutar flujo.

4. Cuando la ejecución del flujo se inicie correctamente (indicado por una marca de verificación verde), seleccione Listo.
<img width="358" height="155" alt="image" src="https://github.com/user-attachments/assets/208336ce-957f-4826-aa85-68146d3e451e" />

Cuando el flujo termine de ejecutarse, aparecerá el mensaje El flujo se ejecutó correctamente en color verde en la parte superior.

5. Para mostrar el flujo, salga del diseñador seleccionando Atrás (flecha a la izquierda) en la esquina superior izquierda, debajo de la Power Automate barra de título (no el botón Atrás de la barra de direcciones).

6, La pantalla que aparece muestra los detalles del flujo que creó, incluido el propietario, la fecha de creación, el tipo de flujo, las conexiones y otra información sobre el flujo.

En el panel Historial de ejecución de 28 días, puede comprobar si el flujo se ejecutó correctamente, si tuvo un error o si todavía se está ejecutando.

<img width="1471" height="550" alt="image" src="https://github.com/user-attachments/assets/b3dd3cba-be80-4166-90e7-0c6284a18b8f" />

## Ejecute su flujo de nube
Cuando el flujo de nube se ejecuta correctamente, aparece en la lista Mis flujos. Aquí es donde puede ejecutarlo.

1. En el menú de navegación de la izquierda, seleccione Mis flujos. El flujo de nube está en la parte superior de la lista.

2. Pase el cursor sobre el flujo de nube y seleccione el icono Ejecutar (el primer icono, que es un triángulo que apunta hacia la derecha).

<img width="1100" height="220" alt="image" src="https://github.com/user-attachments/assets/0256dfa7-1d0e-4fdf-ab16-059d4e9d05a1" />

En el panel Ejecutar flujo, seleccione Ejecutar flujo.

3. Cuando la ejecución del flujo se inicie correctamente (indicado por una marca de verificación verde), seleccione Listo.

4. Cuando el flujo termina de ejecutarse, envía un correo electrónico a la dirección que ha especificado en el campo Para. En este tutorial, ha utilizado su propio correo electrónico.

5. Compruebe la bandeja de entrada de su correo electrónico para ver el correo electrónico que le envió el flujo de nube.

Enhorabuena. Ha creado correctamente un flujo de nube, lo ha probado y lo ha ejecutado.
