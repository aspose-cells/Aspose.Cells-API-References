---
title: "Clase WebQueryConnection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ExternalConnections.WebQueryConnection. Especifica las propiedades para una fuente de consulta web. Una consulta web recuperará datos de tablas HTML y también puede proporcionar parámetros HTTP Get para que el servidor web los procese al generar el HTML, incluyendo los parámetros y los elementos de parámetros."
type: docs
url: /es/net/aspose.cells.externalconnections/webqueryconnection/
---
## WebQueryConnection class

Especifica las propiedades para una fuente de consulta web. Una consulta web recuperará datos de tablas HTML y también puede suministrar parámetros HTTP "Get" para ser procesados por el servidor web al generar el HTML, incluyendo los parámetros y los elementos de parámetro.

```csharp
public class WebQueryConnection : ExternalConnection
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Indica si la conexión puede actualizarse en segundo plano (asíncronamente). true si el uso preferido de la conexión es actualizar asíncronamente en segundo plano; false si el uso preferido es actualizar sincrónicamente en primer plano.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/webqueryconnection/classtype/) { get; } | Obtiene el tipo de este objeto [`ExternalConnection`](../externalconnection/). |
| virtual [Command](../../aspose.cells.externalconnections/externalconnection/command/) { get; set; } | La cadena que contiene el comando de base de datos para pasar a la API del proveedor de datos que interactuará con la fuente externa para recuperar datos (Hereda de [`ExternalConnection`](../externalconnection/).) |
| virtual [CommandType](../../aspose.cells.externalconnections/externalconnection/commandtype/) { get; set; } | Especifica el tipo de comando OLE DB. 1. La consulta especifica un nombre de cubo 2. La consulta especifica una instrucción SQL 3. La consulta especifica un nombre de tabla 4. La consulta especifica que se ha proporcionado información predeterminada, y depende del proveedor interpretarla. 5. La consulta se realiza contra un proveedor de datos de lista basado en la web. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Especifica la descripción del usuario para esta conexión(Heredado de [`ExternalConnection`](../externalconnection/).) |
| override [ConnectionFile](../../aspose.cells.externalconnections/webqueryconnection/connectionfile/) { get; } | Obtiene el archivo de conexión. |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Especifica el identificador único de esta conexión.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionString](../../aspose.cells.externalconnections/externalconnection/connectionstring/) { get; set; } | La cadena de información de conexión se utiliza para establecer contacto con una fuente de datos OLE DB o ODBC. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Especifica el método de autenticación que se usará al establecer (o restablecer) la conexión.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Especifica el método de autenticación que se usará al establecer (o restablecer) la conexión.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| [EditPage](../../aspose.cells.externalconnections/webqueryconnection/editpage/) { get; set; } | (**Obsoleto.**) La URL de la página web orientada al usuario que muestra los datos de la consulta web. Esta URL se conserva en el caso de que sourceData="true" y la url haya sido redirigida para referenciar un archivo XML. Entonces la página orientada al usuario puede mostrarse en la interfaz y los datos XML pueden recuperarse en segundo plano. |
| [EditWebPage](../../aspose.cells.externalconnections/webqueryconnection/editwebpage/) { get; set; } | La URL de la página web orientada al usuario que muestra los datos de la consulta web. Esta URL se conserva en el caso de que sourceData="true" y la url haya sido redirigida para referenciar un archivo XML. Entonces la página orientada al usuario puede mostrarse en la interfaz y los datos XML pueden recuperarse en segundo plano. |
| [HtmlFormat](../../aspose.cells.externalconnections/webqueryconnection/htmlformat/) { get; set; } | Cómo manejar el formato del origen HTML al incorporar datos de consulta web en la hoja de cálculo. Relevante cuando sourceData es True. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Obtiene el id de la conexión.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| [IsConsecutive](../../aspose.cells.externalconnections/webqueryconnection/isconsecutive/) { get; set; } | Indicador que indica si los delimitadores consecutivos deben tratarse como un solo delimitador. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Indica si la conexión del libro de trabajo asociada ha sido eliminada. true si la conexión ha sido eliminada; de lo contrario, false.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| [IsHtmlTables](../../aspose.cells.externalconnections/webqueryconnection/ishtmltables/) { get; set; } | Indicador que indica si las consultas web deben funcionar solo en tablas HTML. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True si la conexión no se ha actualizado por primera vez; de lo contrario, false. Este estado puede ocurrir cuando el usuario guarda el archivo antes de que una consulta haya terminado de devolver resultados.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| [IsParsePre](../../aspose.cells.externalconnections/webqueryconnection/isparsepre/) { get; set; } | Indicador que indica si los datos contenidos dentro de etiquetas HTML PRE en la página web se analizan en columnas al importar la página a una tabla de consulta. |
| [IsSameSettings](../../aspose.cells.externalconnections/webqueryconnection/issamesettings/) { get; set; } | Indicador que indica si se deben analizar todas las tablas dentro de un bloque PRE con la misma configuración de ancho que la primera fila. |
| [IsTextDates](../../aspose.cells.externalconnections/webqueryconnection/istextdates/) { get; set; } | Indicador que indica si las fechas deben importarse a las celdas de la hoja de cálculo como texto en lugar de como fechas. |
| [IsXl2000](../../aspose.cells.externalconnections/webqueryconnection/isxl2000/) { get; set; } | Esta bandera existe por compatibilidad hacia atrás con archivos de hoja de cálculo más antiguos existentes, y se establece en true si esta consulta web se actualizó en una aplicación de hoja de cálculo más reciente o igual a Microsoft Excel 2000. Este es un atributo opcional que puede ser ignorado. |
| [IsXl97](../../aspose.cells.externalconnections/webqueryconnection/isxl97/) { get; set; } | Esta bandera existe por compatibilidad hacia atrás con archivos de hoja de cálculo más antiguos existentes, y se establece en true si esta consulta web se creó en Microsoft Excel 97. Este es un atributo opcional que puede ser ignorado. |
| [IsXml](../../aspose.cells.externalconnections/webqueryconnection/isxml/) { get; set; } | true si la fuente de la consulta web es XML (en lugar de HTML), de lo contrario false. |
| [IsXmlSourceData](../../aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata/) { get; set; } | Bandera que indica que los datos de origen XML deben importarse en lugar de la tabla HTML misma. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True cuando la aplicación de hoja de cálculo debe intentar mantener la conexión abierta. Cuando false, la aplicación debe cerrar la conexión después de recuperar la información.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Especifica el nombre de la conexión. Cada conexión debe tener un nombre único.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Especifica la ruta completa al archivo de conexión externa desde el cual se creó esta conexión. Si una conexión falla durante un intento de actualizar datos, y reconnectionMethod=1, entonces la aplicación de hoja de cálculo volverá a intentarlo usando la información del archivo de conexión externa en lugar del objeto de conexión incrustado en el libro. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Indica si la aplicación de hoja de cálculo debe siempre y únicamente usar la información de conexión en el archivo de conexión externa indicado por el atributo odcFile cuando se actualiza la conexión. Si es falso, entonces la aplicación de hoja de cálculo debe seguir el procedimiento indicado por el atributo reconnectionMethod (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Obtiene [`ConnectionParameterCollection`](../connectionparametercollection/) para una consulta ODBC o web. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [Post](../../aspose.cells.externalconnections/webqueryconnection/post/) { get; set; } | Devuelve o establece la cadena utilizada con el método post para enviar datos a un servidor web y obtener datos de una consulta web. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula/) { get; } | Obtiene la definición de la fórmula de Power Query. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsoleto.**) Especifica lo que la aplicación de hoja de cálculo debe hacer cuando una conexión falla. El valor predeterminado es ReConnectionMethodType.Required. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Especifica lo que la aplicación de hoja de cálculo debe hacer cuando una conexión falla. El valor predeterminado es ReConnectionMethodType.Required. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Especifica el número de minutos entre actualizaciones automáticas de la conexión. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | Verdadero si esta conexión debe actualizarse al abrir el archivo; de lo contrario, falso. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | Verdadero si los datos externos obtenidos a través de la conexión para rellenar una tabla deben guardarse con el libro; de lo contrario, falso. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | Verdadero si la contraseña debe guardarse como parte de la cadena de conexión; de lo contrario, Falso. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| virtual [SecondCommand](../../aspose.cells.externalconnections/externalconnection/secondcommand/) { get; set; } | Especifica una segunda cadena de texto de comando que se conserva cuando los campos de página basados en servidor de PivotTable están en uso. Para conexiones ODBC, serverCommand suele ser una consulta más amplia que command (no hay cláusula WHERE presente en la primera). Basado en estos 2 comandos (Command y ServerCommand), la interfaz de usuario de parámetros puede poblarse y pueden construirse consultas parametrizadas (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Se usa cuando la fuente de datos externa es basada en archivos. Cuando una conexión a dicha fuente de datos falla, la aplicación de hoja de cálculo intenta conectarse directamente a este archivo. Puede expresarse en notación de URI o ruta de archivo específica del sistema. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Obtiene o establece el tipo DataSource de la conexión externa. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Identificador para Single Sign On (SSO) usado para la autenticación entre un servidor intermedio spreadsheetML y la fuente de datos externa. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsoleto.**) Obtiene o establece el tipo DataSource de la conexión externa. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [Url](../../aspose.cells.externalconnections/webqueryconnection/url/) { get; set; } | URL a usar para actualizar datos externos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassWebQueryConnectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();

            try
            {
                // Crear conexión de consulta web a través de la colección
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];
                
                connection.Url = "https://example.com/financial-data";
                connection.IsHtmlTables = true;
                connection.IsTextDates = true;
                connection.HtmlFormat = HtmlFormatHandlingType.All;

                Console.WriteLine($"Web query URL: {connection.Url}");
                Console.WriteLine($"HTML tables only: {connection.IsHtmlTables}");

                workbook.Save("WebQueryConnectionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebQueryConnection: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


