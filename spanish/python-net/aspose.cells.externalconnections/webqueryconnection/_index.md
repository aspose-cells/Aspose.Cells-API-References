---
title: WebQueryConnection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 70
url: /es/python-net/aspose.cells.externalconnections/webqueryconnection/
is_root: false
---
##  WebQueryConnection clase
 Una consulta web recuperará datos de las tablas HTML,
 y también puede proporcionar parámetros HTTP "Get" para que los procese el servidor web al generar el HTML por
incluidos los parámetros y elementos de parámetro.



**Herencia:** [WebQueryConnection](/cells/python-net/aspose.cells.externalconnections/webqueryconnection) → 
[ExternalConnection](/cells/es/python-net/aspose.cells.externalconnections/externalconnection)



El tipo WebQueryConnection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [id](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/id) | Obtiene el id de la conexión.|
| [power_query_formula](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/power_query_formula) | Obtiene la definición de la fórmula de consulta de potencia.|
| [type](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/type) | Obtiene o establece el tipo de origen de datos de la conexión externa.|
| [source_file](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/source_file) | Se utiliza cuando la fuente de datos externa está basada en archivos.<br/> fuente falla, la aplicación de hoja de cálculo intenta conectarse directamente a este archivo.<br/> expresado en URI o notación de ruta de archivo específica del sistema.|
| [sso_id](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/sso_id) | Identificador de inicio de sesión único (SSO) utilizado para la autenticación entre un intermediario<br/> servidor spreadsheetML y la fuente de datos externa.|
| [save_password](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/save_password) | True si la contraseña se guardará como parte de la cadena de conexión; de lo contrario, False.|
| [save_data](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/save_data) | True si se van a guardar los datos externos obtenidos a través de la conexión para completar una tabla<br/> con el libro de trabajo; de lo contrario, falso.|
| [refresh_on_load](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_on_load) | True si esta conexión debe actualizarse al abrir el archivo;|
| [reconnection_method_type](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method_type) | Especifica lo que debe hacer la aplicación de hoja de cálculo cuando falla una conexión.<br/>El valor predeterminado es ReConnectionMethodType.Required.|
| [reconnection_method](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method) | Especifica lo que debe hacer la aplicación de hoja de cálculo cuando falla una conexión.<br/>El valor predeterminado es ReConnectionMethodType.Required.|
| [only_use_connection_file](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/only_use_connection_file) | Indica si la aplicación de hoja de cálculo debe usar siempre y solo el<br/> información de conexión en el archivo de conexión externo indicado por el atributo odcFile<br/> cuando se actualiza la conexión. Si es falso, la aplicación de hoja de cálculo<br/> debe seguir el procedimiento indicado por el atributo reconnectionMethod|
| [odc_file](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/odc_file) | Especifica la ruta completa al archivo de conexión externa desde el que se realizó esta conexión.<br/> Si una conexión falla durante un intento de actualizar los datos y reconnectionMethod=1,<br/> luego, la aplicación de hoja de cálculo volverá a intentarlo utilizando la información del archivo de conexión externa<br/> en lugar del objeto de conexión incrustado en el libro de trabajo.|
| [is_new](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/is_new) | True si la conexión no se ha actualizado por primera vez; de lo contrario, false.<br/> Este estado puede ocurrir cuando el usuario guarda el archivo antes de que termine de regresar una consulta.|
| [name](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/name) | Especifica el nombre de la conexión.|
| [keep_alive](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/keep_alive) | Verdadero cuando la aplicación de hoja de cálculo debe esforzarse por mantener la conexión<br/>Cuando es falso, la aplicación debe cerrar la conexión después de recuperar el<br/> información.|
| [refresh_internal](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_internal) | Especifica la cantidad de minutos entre actualizaciones automáticas de la conexión.|
| [connection_id](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/connection_id) | Especifica el identificador único de esta conexión.|
| [connection_description](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/connection_description) | Especifica la descripción del usuario para esta conexión.|
| [is_deleted](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/is_deleted) |Indica si se eliminó la conexión del libro de trabajo asociado.<br/> en caso contrario, falso.|
| [credentials_method_type](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/credentials_method_type) | Especifica el método de autenticación que se utilizará al establecer (o restablecer) la conexión.|
| [credentials](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/credentials) | Especifica el método de autenticación que se utilizará al establecer (o restablecer) la conexión.|
| [background_refresh](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/background_refresh) | Indica si la conexión se puede actualizar en segundo plano (asincrónicamente).<br/>true si el uso preferido de la conexión es actualizar de forma asíncrona en segundo plano;<br/> falso si el uso preferido de la conexión es actualizar sincrónicamente en primer plano.|
| [parameters](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/parameters) | Obtiene [ConnectionParameterCollection](/cells/es/python-net/aspose.cells.externalconnections/connectionparametercollection) para una consulta web o ODBC.|
| [is_xml](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml) | verdadero si el origen de la consulta web es XML (frente a HTML); de lo contrario, falso.|
| [is_xl97](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl97) |Esta marca existe para la compatibilidad con versiones anteriores de archivos de hojas de cálculo existentes más antiguos y se establece<br/>a verdadero si esta consulta web se creó en Microsoft Excel 97.<br/> Este es un atributo opcional que se puede ignorar.|
| [is_xl2000](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl2000) |Esta marca existe para la compatibilidad con versiones anteriores de archivos de hojas de cálculo existentes más antiguos y se establece<br/>verdadero si esta consulta web se actualizó en una aplicación de hoja de cálculo más reciente o igual<br/>al Microsoft excel 2000.<br/> Este es un atributo opcional que se puede ignorar.|
| [url](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/url) | URL que se usará para actualizar los datos externos.|
| [is_text_dates](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/is_text_dates) | Marca que indica si las fechas deben importarse a las celdas de la hoja de trabajo como texto en lugar de fechas.|
| [is_xml_source_data](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml_source_data) | Indicador que indica que los datos de origen XML deben importarse en lugar de la propia tabla HTML.|
| [post](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/post) | Devuelve o establece la cadena utilizada con el método de publicación para ingresar datos en un servidor web<br/> para devolver datos de una consulta web.|
| [is_parse_pre](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/is_parse_pre) | Bandera que indica si los datos contenidos dentro de las etiquetas PRE HTML en la página web son<br/> se analiza en columnas cuando importa la página a una tabla de consulta.|
| [is_html_tables](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/is_html_tables) | Indicador que indica si las consultas web solo deben funcionar en las tablas HTML.|
| [html_format](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/html_format) | Cómo manejar el formato de la fuente HTML al traer datos de consultas web al<br/> hoja de trabajo. Relevante cuando sourceData es True.|
| [is_same_settings](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/is_same_settings) |Indicador que indica si analizar todas las tablas dentro de un bloque PRE con la misma configuración de ancho<br/> como la primera fila.|
| [edit_web_page](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/edit_web_page) | La URL de la página web orientada al usuario que muestra los datos de la consulta web.<br/>en el caso de que sourceData="true" y url hayan sido redirigidos para hacer referencia a un archivo XML.<br/>Luego, la página orientada al usuario se puede mostrar en la interfaz de usuario y los datos XML se pueden recuperar.<br/> entre bastidores.|
| [edit_page](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/edit_page) | La URL de la página web orientada al usuario que muestra los datos de la consulta web.<br/>en el caso de que sourceData="true" y url hayan sido redirigidos para hacer referencia a un archivo XML.<br/>Luego, la página orientada al usuario se puede mostrar en la interfaz de usuario y los datos XML se pueden recuperar.<br/> entre bastidores.|
| [is_consecutive](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection/is_consecutive) | Indicador que indica si los delimitadores consecutivos deben tratarse como un solo delimitador.|



###  Ver también
* módulo [aspose.cells.externalconnections](..)
* clase [ConnectionParameterCollection](/cells/es/python-net/aspose.cells.externalconnections/connectionparametercollection)
* clase [ExternalConnection](/cells/es/python-net/aspose.cells.externalconnections/externalconnection)
* clase [WebQueryConnection](/cells/es/python-net/aspose.cells.externalconnections/webqueryconnection)
