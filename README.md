# Azure-QnA-Bot
Creación de Bot para QnA en Azure

![Logo de QnA](https://github.com/AlanAlvaradoR/Azure-QnA-Bot/blob/main/imagenes/QnA.jpg)

## Requisitos

- Cuenta de [Azure](https://portal.azure.com/) con suscripción activa
- Computadora con Windows, Linux o MacOs

---------------------------------------------------------

## Pasos

1. Se inicia sesión en la página de [QnA de Azure](https://www.qnamaker.ai/)

2. Se crea una nueva "knowledge base".

3. Se da click en "Create a QnA Service"

4. Se nos redigirá al portal de Azure donde debemos llenar los parámetros requeridos para crear el recurso, una vez llenos los parámetros necearios se da click en "revisar y crear"

5. Se validarán los datos para poder activar la opción de "crear". Una vez activada se da click en ella y se espera que termine la implementación.

6. Se crearán varios recursos, se recomienda esperar al menos 10min para seguir con el siguiente paso.

![QnA1](https://github.com/AlanAlvaradoR/Azure-QnA-Bot/blob/main/imagenes/QnA1.PNG)

7. Se regresa a la página de QnA Maker y se da click en "refresh", debería abrir unos nuevos parámetros como los siguientes:

![QnA2](https://github.com/AlanAlvaradoR/Azure-QnA-Bot/blob/main/imagenes/QnA2.PNG)

8. Se rellenan los parámetros (suscripción, servicio y lenguaje)

9. Se le da un nombre al bot (Step 3: Name your KB)

10. En el Step 4 se puede seleccionar una URL o un archivo local donde ya se tenga precargadas las preguntas y respuestas que se requieran. Más abajo también es posible asignar un tipo de voz para las respuestas de voz. Si no se tiene un archivo o URL para este apartado, simplemente se deja en blanco, más adelante se pueden llenar las preguntas y respuestas de formas manual.

11. Se da click en "Create your KB" y se espera a que termine.

12. Una vez terminado mostrará un menú como el siguiente:

![QnA3](https://github.com/AlanAlvaradoR/Azure-QnA-Bot/blob/main/imagenes/QnA3.PNG)

13. Se da click en "Add QnA Pair"

14. Se abrirá una nueva pregunta en la parte inferior, en el lado izquierdo se debe escribir la pregunta, frase u oración que se espera que diga el usuario, del lado derecho se debe poner la respuesta que debe dar el bot.

**NOTA:** Si hay varias opciones al texto que manda el usuario, se puede dar click en "Add alternative phrasing" para agregar más opciones del mismo texto o que lleven la misma respuesta.

15. Si se desea agregar más preguntas y respuestas diferentes, se repiten los pasos 13 y 14. También se pueden agregar links clickeables e imagenes de la web a la respuestas del bot por medio del botón de tres puntos.

16. Una vez se hayan terminado de redactar todas las respuestas y preguntas, se da click en "Save and train" en la parte superior. Se espera a que termine.

**NOTA:** Si se modifica alguna pregunta o respuestas, siempre es necesario repetir el paso 16 para que los cambios surtan efecto.

17. Si se desea probar el funcionamiento antes de ponerlo a funcionar, se da click en "Test" en la parte superior derecha y se iniciará una conversación de prueba con el bot.

18. Dentro de la conversación de prueba con el bot, se pueden identificar fallos en respuestas, al detectar preguntar y más. Si se desea analizar una pregunta o texto en especial introducido por el usuario, se da click en "Inspect" debajo del texto en cuestión para ver sus detalles.

19. Una vez que se ha probado y se detemrina que esta listo, se da click en la pestaña superior "Publish" y después en el botón "Publish".

20. Se dará instrucciones para usarlo por medio de un https, si se desea se puede usar mediante un recurso de Azure al hacer click en "Create Bot".

21. Se abrirá el portal de Azure donde se deben llenar los parámetros requeridos y seleccionar el idioma del SDK (C# o Node.js) y se da click en "Crear"

**NOTA:** Si no deja crear el recurso, es probable que sea error de Azure, se debe seleccionar de nuevo la suscripción o recargar de nuevo la página para poder proseguir.

22. Si se desea modificar alguna pregunta o respuesta, se puede ir de nuevo a la página de [QnA de Azure](https://www.qnamaker.ai/), buscar el "Knowledge base" que nos interese, seleccionarlo, modificar lo que se necesite, darle click en "Save and train" y luego en "Publish".

23. En el portal de Azure al finalizar la implementación de los recursos se mostrará un menú como el siguiente y se da click en "ir al recurso"

![QnA4](https://github.com/AlanAlvaradoR/Azure-QnA-Bot/blob/main/imagenes/QnA4.PNG)

24. Después se selecciona en el menú lateral izquierdo "probar en el chat en web" para probar el buen funcionamiento del bot por medio de un chat de prueba.

**NOTA:** Si por alguna razón no funciona la primera vez, es necesario volver a crear un nuevo recurso de Azure para el bot y repetir la configuración en el portal de Azure.

25. Una vez se prueba el buen funcionamiento, se da click en el menú lateral izquierdo en "Canales", desde aquí se puede conectar el bot con diferentes plataformas (Telegram, instagram, facebook, etc.), se selecciona la plataforma que se quiera y se siguen los pasos allí estipulados para ocnectar el bot.


