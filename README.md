##Descarga y configuración inicial
Tras hacer click en el archivo "Digitalus Xtractor.xlsm", pulse el botón "Download raw file".
<img width="2147" height="537" alt="image" src="https://github.com/user-attachments/assets/82876ca3-d178-416e-8645-97e2791d354e" />

Una vez descargado, haga click derecho sobre el archivo y en propiedades active "Unblock" y después aplique los cambios. Esto es necesario porque Windows bloquea por defecto los archivos macro (.xlsm) descargados de Internet.
<img width="768" height="955" alt="image" src="https://github.com/user-attachments/assets/2598978b-e26e-4609-accc-3430e76ae9b2" />
Nota: La primera vez que abra el archivo saldrá un aviso de seguridad, con pulsar "Enable Content" ya no debiera volver a salir.

Si tiene las macros desactivadas por defecto, debe acceder a "File > Options > Trust Center > Trust Center Settings…"
<img width="886" height="401" alt="image" src="https://github.com/user-attachments/assets/1ee5b4c5-8750-4864-88e2-7bddbf3788b0" />

Desde el menú izquierdo seleccione "Macro Settings" y active las macros.
<img width="886" height="530" alt="image" src="https://github.com/user-attachments/assets/2c0e75f0-2a91-49fb-a243-95641550520c" />

##Crear API Key de Google Gemini
A través de la siguiente url, acceda con su cuenta de Google y pulse en "Crear clave de API".
https://aistudio.google.com/api-keys
Nota: Si no dispone de ningún proyecto precio le requerirá generarlo en unos sencillos pasos.

Una vez obtenga la clave API, haga copiar/pegar dentro del campo definido en la pestaña "Config" de la herramienta.
<img width="678" height="582" alt="image" src="https://github.com/user-attachments/assets/170a9707-ed2f-4dda-90e5-b1d482149a4f" />

#Configuración de extracción y Uso
- Si tras pulsar el botón "Obtener modelos IA" no obtiene ningún error es que la API Key funciona correctamente. En este momento se recomienda guardar el archivo para que la API Key quede predefinida para un uso posterior.
- Desde el desplegable "Modelos" puede elegir el modelo de IA a utilizar en la extracción de datos aunque se recomienda usar una versión flash como la 2.5 debido al consumo de tokens, sobre todo si usa un plan gratuito.
- En caso de trabajar con una gran cantidad de facturas diariamente o requerir un modelo superior por la complejidad de las mismas, se recomienda utilizar una API Key de pago con el modelo que mejor se ajuste a sus necesidades.
- La configuración está predefinida para capturar 10 campos. Puede editar sus identificadores y nombres de columna, así como activar o desactivar la extracción de un campo concreto. Si en el campo "Extraer" hay una "X" entonces el sistema procederá a su extracción.
- En la columna formato se puede definir un formato según la nomenclatura de Excel en aquellos casos que se requiera.

Una vez esté todo a gusto el usuario, solo debe pulsar "iniciar captura de datos" y elegir la carpeta donde tiene las facturas a procesar.
Según el rendimiento de su ordenador es posible que en algunos momentos el programa se sature por el esfuerzo de la ejecución del proceso, tan solo debe ser paciente y esperar a que termine.
Una vez finalizado, los datos quedarán automáticamente extraídos en la pestaña "Xtractor".
Nota 1: En caso de procesar gran cantidad de facturas a la vez, es posible que se alcancen los límites de la API Key de Gemini; en ese caso se obtendrá un error indicando dicha situación y se mostrarán los datos de facturas procesadas hasta ese momento.
Nota 2: Los límites de la API Key gratuita se reinician diariamente por lo que una vez falle tan solo debe esperar al día siguiente para continuar a no ser que prefiera usar API Key de pago.

## Aviso legal y de uso

### Precisión de los datos extraídos
Esta herramienta utiliza un modelo de IA (Google Gemini) para leer e interpretar 
facturas. Los modelos de IA pueden cometer errores de lectura, especialmente en 
documentos de baja calidad, formatos poco habituales o campos ambiguos.

**Revisa siempre los datos extraídos antes de usarlos en contabilidad, 
declaraciones fiscales o cualquier proceso con implicaciones legales o 
económicas.** La herramienta es un acelerador, no un sustituto de la 
verificación humana.

### Flujo y privacidad de los datos
Digitalus Xtractor no envía tus datos a ningún servidor de Digitalus Solutions. 
El contenido de las facturas se envía directamente desde tu equipo a la API de 
Google Gemini, usando tu propia clave de API. Ni el autor ni Digitalus Solutions 
tienen acceso a los documentos que proceses.

**Importante:** si usas una clave de API en el nivel gratuito de Google, sus 
términos de servicio permiten que el contenido enviado (incluidos archivos e 
imágenes) se use para mejorar sus productos, y puede ser revisado por personal 
de Google. Si vas a procesar facturas con datos personales de clientes o 
proveedores, revisa los [términos actuales de la API de Gemini](https://ai.google.dev/gemini-api/terms) 
y valora usar el nivel de pago, que no tiene este uso de datos.

### Sin garantías
Esta herramienta se proporciona "tal cual" (as-is), sin garantía de ningún tipo, 
explícita o implícita, incluyendo pero sin limitarse a garantías de 
comerciabilidad, idoneidad para un propósito concreto o ausencia de errores. 
El autor no se responsabiliza de pérdidas, daños o decisiones tomadas a partir 
de los datos generados por esta herramienta. El uso es bajo tu propia 
responsabilidad.
