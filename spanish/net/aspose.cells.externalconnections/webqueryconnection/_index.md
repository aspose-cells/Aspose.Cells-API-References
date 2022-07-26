---
title: WebQueryConnection
second_title: Referencia de API de Aspose.Cells para .NET
description: Especifica las propiedades de un origen de consulta web. Una consulta web recuperará datos de tablas HTML y también puede proporcionar parámetros HTTP Get para que los procese el servidor web al generar el HTML mediante  incluidos los parámetros y elementos de parámetro.
type: docs
weight: 3350
url: /es/net/aspose.cells.externalconnections/webqueryconnection/
---
## WebQueryConnection class

Especifica las propiedades de un origen de consulta web. Una consulta web recuperará datos de tablas HTML, y también puede proporcionar parámetros HTTP "Get" para que los procese el servidor web al generar el HTML mediante , incluidos los parámetros y elementos de parámetro.

```csharp
public class WebQueryConnection : ExternalConnection
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh) { get; set; } | Indica si la conexión se puede actualizar en segundo plano (asincrónicamente). verdadero si el uso preferido de la conexión es actualizar de forma asíncrona en segundo plano; falso si el uso preferido de la conexión es actualizar sincrónicamente en primer plano. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription) { get; set; } | Especifica la descripción de usuario para esta conexión |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid) { get; } | Especifica el identificador único de esta conexión. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype) { get; set; } | Especifica el método de autenticación que se utilizará al establecer (o restablecer) la conexión. |
| [EditWebPage](../../aspose.cells.externalconnections/webqueryconnection/editwebpage) { get; set; } | La URL de la página web orientada al usuario que muestra los datos de la consulta web. Esta URL persiste en el caso de que sourceData="true" y la URL se hayan redirigido para hacer referencia a un archivo XML. Luego, la página orientada al usuario se puede mostrar en la interfaz de usuario y los datos XML se pueden recuperar detrás de escena. |
| [HtmlFormat](../../aspose.cells.externalconnections/webqueryconnection/htmlformat) { get; set; } | Cómo manejar el formato de la fuente HTML al traer datos de consultas web a la hoja de trabajo . Relevante cuando sourceData es True. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id) { get; } | Obtiene el id de la conexión. |
| [IsConsecutive](../../aspose.cells.externalconnections/webqueryconnection/isconsecutive) { get; set; } | Indicador que indica si los delimitadores consecutivos deben tratarse como un solo delimitador. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted) { get; set; } | Indica si se eliminó la conexión del libro de trabajo asociado. true si se ha eliminado la conexión ; de lo contrario, false. |
| [IsHtmlTables](../../aspose.cells.externalconnections/webqueryconnection/ishtmltables) { get; set; } | Indicador que indica si las consultas web solo deben funcionar en tablas HTML. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew) { get; set; } | True si la conexión no se ha actualizado por primera vez; en caso contrario, falso. Este estado puede ocurrir cuando el usuario guarda el archivo antes de que una consulta haya terminado de regresar. |
| [IsParsePre](../../aspose.cells.externalconnections/webqueryconnection/isparsepre) { get; set; } | Indicador que indica si los datos contenidos en las etiquetas HTML PRE de la página web se analizan en columnas cuando importa la página a una tabla de consulta. |
| [IsSameSettings](../../aspose.cells.externalconnections/webqueryconnection/issamesettings) { get; set; } | Indicador que indica si analizar todas las tablas dentro de un bloque PRE con la misma configuración de ancho que la primera fila. |
| [IsTextDates](../../aspose.cells.externalconnections/webqueryconnection/istextdates) { get; set; } | Indicador que indica si las fechas deben importarse a las celdas de la hoja de trabajo como texto en lugar de fechas. |
| [IsXl2000](../../aspose.cells.externalconnections/webqueryconnection/isxl2000) { get; set; } | Este indicador existe para la compatibilidad con versiones anteriores de archivos de hojas de cálculo existentes más antiguos, y se establece en verdadero si esta consulta web se actualizó en una aplicación de hoja de cálculo más reciente o igual a Microsoft Excel 2000. Este es un atributo opcional que se puede ignorar. |
| [IsXl97](../../aspose.cells.externalconnections/webqueryconnection/isxl97) { get; set; } | Esta marca existe para la compatibilidad con versiones anteriores de archivos de hojas de cálculo existentes más antiguos, y se establece en verdadero si esta consulta web se creó en Microsoft Excel 97. Este es un atributo opcional que se puede ignorar. |
| [IsXml](../../aspose.cells.externalconnections/webqueryconnection/isxml) { get; set; } | verdadero si el origen de la consulta web es XML (frente a HTML); de lo contrario, falso. |
| [IsXmlSourceData](../../aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata) { get; set; } | Indicador que indica que los datos de origen XML deben importarse en lugar de la propia tabla HTML. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive) { get; set; } | Verdadero cuando la aplicación de hoja de cálculo debe esforzarse por mantener abierta la conexión . Cuando es falso, la aplicación debe cerrar la conexión después de recuperar la información . |
| [Name](../../aspose.cells.externalconnections/externalconnection/name) { get; set; } | Especifica el nombre de la conexión. Cada conexión debe tener un nombre único. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile) { get; set; } | Especifica la ruta completa al archivo de conexión externa a partir del cual se creó esta conexión . Si falla una conexión durante un intento de actualizar los datos y reconnectionMethod=1, , la aplicación de hoja de cálculo volverá a intentarlo utilizando la información del archivo de conexión externo en lugar del objeto de conexión incrustado en el libro de trabajo. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile) { get; set; } | Indica si la aplicación de hoja de cálculo debe usar siempre y solo la información de conexión en el archivo de conexión externo indicado por el atributo odcFile cuando se actualiza la conexión. Si es falso, la aplicación de hoja de cálculo debe seguir el procedimiento indicado por el atributo reconnectionMethod |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters) { get; } | Obtiene[`ConnectionParameterCollection`](../connectionparametercollection) para una consulta ODBC o web. |
| [Post](../../aspose.cells.externalconnections/webqueryconnection/post) { get; set; } | Devuelve o establece la cadena utilizada con el método de publicación para ingresar datos en un servidor web para devolver datos de una consulta web. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula) { get; } | Obtiene la definición de la fórmula power query. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype) { get; set; } | Especifica qué debe hacer la aplicación de hoja de cálculo cuando falla una conexión. El valor predeterminado es ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal) { get; set; } | Especifica la cantidad de minutos entre actualizaciones automáticas de la conexión. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload) { get; set; } | True si esta conexión debe actualizarse al abrir el archivo; de lo contrario, false. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata) { get; set; } | Verdadero si los datos externos obtenidos a través de la conexión para completar una tabla deben guardarse con el libro de trabajo; en caso contrario, falso. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword) { get; set; } | True si la contraseña se guardará como parte de la cadena de conexión; de lo contrario, Falso. |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile) { get; set; } | Se utiliza cuando el origen de datos externo está basado en archivos. Cuando falla una conexión a dicha fuente de datos , la aplicación de hoja de cálculo intenta conectarse directamente a este archivo. Puede ser expresado en URI o notación de ruta de archivo específica del sistema. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid) { get; set; } | Identificador para inicio de sesión único (SSO) utilizado para la autenticación entre un servidor intermedio spreadsheetML y la fuente de datos externa. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type) { get; set; } | Obtiene o establece el tipo de origen de datos de la conexión externa. |
| [Url](../../aspose.cells.externalconnections/webqueryconnection/url) { get; set; } | URL a usar para actualizar datos externos. |

### Ver también

* class [ExternalConnection](../externalconnection)
* espacio de nombres [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
