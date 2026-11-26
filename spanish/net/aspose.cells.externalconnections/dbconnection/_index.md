---
title: "Clase DBConnection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.ExternalConnections.DBConnection class. Especifica todas las propiedades asociadas a una conexión de datos externa ODBC o OLE DB"
type: docs
url: /es/net/aspose.cells.externalconnections/dbconnection/
---
## DBConnection class

Especifica todas las propiedades asociadas a una conexión de datos externa ODBC o OLE DB.

```csharp
public class DBConnection : ExternalConnection
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Indica si la conexión puede actualizarse en segundo plano (asíncronamente). true si el uso preferido de la conexión es actualizar asíncronamente en segundo plano; false si el uso preferido es actualizar sincrónicamente en primer plano.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/dbconnection/classtype/) { get; } | Obtiene el tipo de este objeto [`ExternalConnection`](../externalconnection/). |
| override [Command](../../aspose.cells.externalconnections/dbconnection/command/) { get; set; } | La cadena que contiene el comando de base de datos que se pasa a la API del proveedor de datos que interactuará con la fuente externa para recuperar datos |
| override [CommandType](../../aspose.cells.externalconnections/dbconnection/commandtype/) { get; set; } | Especifica el tipo de comando OLE DB. 1. La consulta especifica un nombre de cubo 2. La consulta especifica una instrucción SQL 3. La consulta especifica un nombre de tabla 4. La consulta indica que se ha proporcionado información predeterminada, y depende del proveedor interpretarla. 5. La consulta se realiza contra un proveedor de datos de lista basado en la web. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Especifica la descripción del usuario para esta conexión(Heredado de [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | Obtiene el archivo de conexión.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Especifica el identificador único de esta conexión.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| [ConnectionInfo](../../aspose.cells.externalconnections/dbconnection/connectioninfo/) { get; set; } | (**Obsolete.**) La cadena de información de conexión se usa para contactar con una fuente de datos OLE DB o ODBC. |
| override [ConnectionString](../../aspose.cells.externalconnections/dbconnection/connectionstring/) { get; set; } | La cadena de información de conexión se usa para contactar con una fuente de datos OLE DB o ODBC. |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Especifica el método de autenticación que se usará al establecer (o restablecer) la conexión.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Especifica el método de autenticación que se usará al establecer (o restablecer) la conexión.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Obtiene el id de la conexión.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Indica si la conexión del libro de trabajo asociada ha sido eliminada. true si la conexión ha sido eliminada; de lo contrario, false.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True si la conexión no se ha actualizado por primera vez; de lo contrario, false. Este estado puede ocurrir cuando el usuario guarda el archivo antes de que una consulta haya terminado de devolver resultados.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True cuando la aplicación de hoja de cálculo debe intentar mantener la conexión abierta. Cuando false, la aplicación debe cerrar la conexión después de recuperar la información.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Especifica el nombre de la conexión. Cada conexión debe tener un nombre único.(Heredado de [`ExternalConnection`](../externalconnection/).) |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Especifica la ruta completa al archivo de conexión externa desde el cual se creó esta conexión. Si una conexión falla durante un intento de actualizar datos, y reconnectionMethod=1, entonces la aplicación de hoja de cálculo volverá a intentarlo usando la información del archivo de conexión externa en lugar del objeto de conexión incrustado en el libro. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Indica si la aplicación de hoja de cálculo debe siempre y únicamente usar la información de conexión en el archivo de conexión externa indicado por el atributo odcFile cuando se actualiza la conexión. Si es falso, entonces la aplicación de hoja de cálculo debe seguir el procedimiento indicado por el atributo reconnectionMethod (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Obtiene [`ConnectionParameterCollection`](../connectionparametercollection/) para una consulta ODBC o web. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| override [PowerQueryFormula](../../aspose.cells.externalconnections/dbconnection/powerqueryformula/) { get; } | Obtiene la definición de la fórmula de Power Query. |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsoleto.**) Especifica lo que la aplicación de hoja de cálculo debe hacer cuando una conexión falla. El valor predeterminado es ReConnectionMethodType.Required. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Especifica lo que la aplicación de hoja de cálculo debe hacer cuando una conexión falla. El valor predeterminado es ReConnectionMethodType.Required. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Especifica el número de minutos entre actualizaciones automáticas de la conexión. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | Verdadero si esta conexión debe actualizarse al abrir el archivo; de lo contrario, falso. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | Verdadero si los datos externos obtenidos a través de la conexión para rellenar una tabla deben guardarse con el libro; de lo contrario, falso. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | Verdadero si la contraseña debe guardarse como parte de la cadena de conexión; de lo contrario, Falso. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| override [SecondCommand](../../aspose.cells.externalconnections/dbconnection/secondcommand/) { get; set; } | Especifica una segunda cadena de texto de comando que se conserva cuando se utilizan campos de página basados en servidor de PivotTable. Para conexiones ODBC, serverCommand suele ser una consulta más amplia que command (no hay cláusula WHERE presente en la primera). Basado en estos 2 comandos (Command y ServerCommand), la interfaz de usuario de parámetros puede poblarse y pueden construirse consultas parametrizadas |
| [SeverCommand](../../aspose.cells.externalconnections/dbconnection/severcommand/) { get; set; } | (**Obsoleto.**) Especifica una segunda cadena de texto de comando que se conserva cuando se utilizan campos de página basados en servidor de PivotTable. Para conexiones ODBC, serverCommand suele ser una consulta más amplia que command (no hay cláusula WHERE presente en la primera). Basado en estos 2 comandos (Command y ServerCommand), la interfaz de usuario de parámetros puede poblarse y pueden construirse consultas parametrizadas |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Se usa cuando la fuente de datos externa es basada en archivos. Cuando una conexión a dicha fuente de datos falla, la aplicación de hoja de cálculo intenta conectarse directamente a este archivo. Puede expresarse en notación de URI o ruta de archivo específica del sistema. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Obtiene o establece el tipo DataSource de la conexión externa. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Identificador para Single Sign On (SSO) usado para la autenticación entre un servidor intermedio spreadsheetML y la fuente de datos externa. (Hereda de [`ExternalConnection`](../externalconnection/).) |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsoleto.**) Obtiene o establece el tipo DataSource de la conexión externa. (Hereda de [`ExternalConnection`](../externalconnection/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassDBConnectionDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea una nueva instancia de DBConnection añadiéndola a la colección
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Establecer propiedades básicas
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";

                // Mostrar propiedades de solo lectura
                Console.WriteLine("DBConnection ClassType: " + dbConnection.ClassType);
                Console.WriteLine("ConnectionString: " + dbConnection.ConnectionString);
                Console.WriteLine("CommandType: " + dbConnection.CommandType);
                Console.WriteLine("Command: " + dbConnection.Command);

                // Guarda el libro de trabajo
                workbook.Save("DBConnectionDemo.xlsx");
                Console.WriteLine("DBConnection demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DBConnection: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


