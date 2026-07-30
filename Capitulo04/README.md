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



### Paso 2 — Flujo de Nube sin Copilot

1. Inicie sesión en Power Automate.

2. En el menú de navegación de la izquierda, seleccione Crear.

3. En Iniciar desde cero, seleccione Flujo de nube programado.

 <img width="760" height="203" alt="image" src="https://github.com/user-attachments/assets/b81d2791-b64b-4042-bac3-26da0bd6ec09" />

4. En el campo Nombre del flujo, escriba un nombre para el flujo. El nombre de la tabla que se usa en este tutorial es Newsletter.

5. En el campo Inicio, seleccione el icono de calendario y, a continuación, seleccione 6/1/25 a las 12:00 AM.

6. En el campo Repetir cada , escriba 1 y, a continuación, seleccione Mes en el menú desplegable.

<img width="1090" height="678" alt="image" src="https://github.com/user-attachments/assets/9fc612a3-3371-44c4-82e1-a82eaf0a32d0" />

7. Seleccione Crear.

El diseñador se abre con el desencadenadorPeriodicidad. Ahora agregará una acción. Un desencadenador es un evento que inicia un flujo de nube. Las Acciones son los eventos que quiere que haga el flujo después de tener lugar el evento desencadenador.

###Complete la creación del flujo de nube

Complete la creación del flujo de nube en el diseñador. Power Automate permite utilizar el nuevo diseñador o el diseñador clásico para configurar el flujo de nubes. Los pasos son similares en ambos diseñadores. Obtenga más información (con ejemplos) sobre el diseñador en Identificar las diferencias entre el diseñador clásico y el diseñador clásico de flujos de nube.

1. Seleccione la ubicación para la nueva acción en el flujo en la nube:

* Nuevo diseñador: seleccione (+) debajo del desencadenador de Periodicidad.
* Diseñador clásico: seleccione + Nuevo paso.

2. Agregue una acción sin enlazar a su flujo de nube:

* Nuevo diseñador: En el campo de búsqueda Agregar una acción, escriba Enviar un correo electrónico (V2) y luego seleccione la acción Enviar un correo electrónico (V2) en Microsoft 365 Outlook.
* Diseñador clásico: en el campo de búsqueda Elegir una operación, escriba Enviar un correo electrónico (V2) y luego seleccione la acción Enviar un correo electrónico (V2) en Microsoft 365 Outlook.

3. Escriba la siguiente información:

a. En el campo Para, introduzca su dirección de correo electrónico.

Si estuvieras haciendo esto en un escenario de la vida real, ingresarías el correo electrónico de la persona a la que deseas enviar el boletín. En este tutorial, se lo envía a usted mismo para que el flujo de nube le envíe el correo electrónico cuando lo ejecute más adelante en este tutorial. También puede enviarlo a varias personas en el campo Para.

b. En el campo Asunto, introduzca El boletín Contoso Cadence.

c. En el campo Cuerpo, copie y pegue lo siguiente:

```powershell
Welcome to the monthly Contoso Cadence newsletter! In this email, you'll find important dates for training sessions and talks. We'll also showcase demos, and list the frequently asked questions for the month.
```

d. Nuevo diseñador: Seleccione (<<) en la esquina superior derecha del panel para contraer el panel de configuración.

Este flujo consta del desencadenador de Recurrencia y la acción Enviar un correo electrónico (V2) que contiene los parámetros establecidos en este procedimiento.

Nuevo
<img width="223" height="207" alt="image" src="https://github.com/user-attachments/assets/067fd3be-13de-4e78-91a5-a1a900fbb494" />

Clásico
<img width="420" height="323" alt="image" src="https://github.com/user-attachments/assets/0d2b34be-43e0-4637-8be7-5fd6cbbd9f86" />

4. Guarde su flujo de nube seleccionando el botón Guardar en la barra de comandos.

Aparece un mensaje verde debajo de la barra de Power Automate título, lo que indica que el flujo se ha guardado.

### Probar su flujo de nube.

1. En la barra de herramientas, seleccione Probar.

2. En el panel Probar el flujo, seleccione Manualmente y, a continuación, Probar.

3. En el panel Ejecutar flujo, seleccione Ejecutar flujo.

4. Cuando la ejecución del flujo se inicie correctamente (indicado por una marca de verificación verde), seleccione Listo.

<img width="358" height="155" alt="image" src="https://github.com/user-attachments/assets/5c54f8bb-97ea-41c6-85bb-6b376c002be0" />

Cuando el flujo termine de ejecutarse, aparecerá el mensaje El flujo se ejecutó correctamente en color verde en la parte superior.

5. Para mostrar el flujo, salga del diseñador seleccionando Atrás (flecha a la izquierda) en la esquina superior izquierda, debajo de la Power Automate barra de título (no el botón Atrás de la barra de direcciones).

La pantalla que aparece muestra los detalles del flujo que creó, incluido el propietario, la fecha de creación, el tipo de flujo, las conexiones y otra información sobre el flujo.

En el panel Historial de ejecución de 28 días, puede comprobar si el flujo se ejecutó correctamente, si tuvo un error o si todavía se está ejecutando.

<img width="1471" height="550" alt="image" src="https://github.com/user-attachments/assets/c8421383-0dfd-4b94-abbd-289929c17e73" />

### Ejecute su flujo de nube

Cuando el flujo de nube se ejecuta correctamente, aparece en la lista Mis flujos. Aquí es donde puede ejecutarlo.

1. En el menú de navegación de la izquierda, seleccione Mis flujos. El flujo de nube está en la parte superior de la lista.

2. Pase el cursor sobre el flujo de nube y seleccione el icono Ejecutar (el primer icono, que es un triángulo que apunta hacia la derecha).

<img width="1100" height="220" alt="image" src="https://github.com/user-attachments/assets/2da4237d-96d9-489c-82ca-3dc6c911ee0c" />


3. En el panel Ejecutar flujo, seleccione Ejecutar flujo.

4. Cuando la ejecución del flujo se inicie correctamente (indicado por una marca de verificación verde), seleccione Listo.

5. Cuando el flujo termina de ejecutarse, envía un correo electrónico a la dirección que ha especificado en el campo Para. En este tutorial, ha utilizado su propio correo electrónico.

6. Compruebe la bandeja de entrada de su correo electrónico para ver el correo electrónico que le envió el flujo de nube.
