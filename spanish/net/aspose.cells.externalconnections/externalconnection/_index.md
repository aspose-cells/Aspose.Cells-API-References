---
title: "Clase ExternalConnection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ExternalConnections.ExternalConnection. Especifica una conexión de datos externa"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/
---
## ExternalConnection class

Especifica una conexión de datos externa

```csharp
public abstract class ExternalConnection
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Indica si la conexión puede actualizarse en segundo plano (asíncronamente). true si el uso preferido de la conexión es actualizar asíncronamente en segundo plano; false si el uso preferido de la conexión es actualizar sincrónicamente en primer plano. |
| abstract [ClassType](../../aspose.cells.externalconnections/externalconnection/classtype/) { get; } | Obtiene el tipo de este objeto `ExternalConnection`. |
| virtual [Command](../../aspose.cells.externalconnections/externalconnection/command/) { get; set; } | La cadena que contiene el comando de base de datos que se pasa a la API del proveedor de datos que interactuará con la fuente externa para recuperar datos |
| virtual [CommandType](../../aspose.cells.externalconnections/externalconnection/commandtype/) { get; set; } | Especifica el tipo de comando OLE DB. 1. La consulta especifica un nombre de cubo 2. La consulta especifica una instrucción SQL 3. La consulta especifica un nombre de tabla 4. La consulta indica que se ha proporcionado información predeterminada, y depende del proveedor interpretarla. 5. La consulta se realiza contra un proveedor de datos de lista basado en la web. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Especifica la descripción del usuario para esta conexión |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | Obtiene el archivo de conexión. |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Especifica el identificador único de esta conexión. |
| virtual [ConnectionString](../../aspose.cells.externalconnections/externalconnection/connectionstring/) { get; set; } | La cadena de información de conexión se usa para contactar con una fuente de datos OLE DB o ODBC. |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Especifica el método de autenticación que se debe usar al establecer (o restablecer) la conexión. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Especifica el método de autenticación que se debe usar al establecer (o restablecer) la conexión. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Obtiene el id de la conexión. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Indica si la conexión del libro de trabajo asociada ha sido eliminada. true si la conexión ha sido eliminada; de lo contrario, false. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True si la conexión no se ha actualizado por primera vez; de lo contrario, false. Este estado puede ocurrir cuando el usuario guarda el archivo antes de que una consulta haya terminado de devolver resultados. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True cuando la aplicación de hoja de cálculo debe esforzarse por mantener la conexión abierta. Cuando false, la aplicación debe cerrar la conexión después de recuperar la información. |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Especifica el nombre de la conexión. Cada conexión debe tener un nombre único. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Especifica la ruta completa al archivo de conexión externa desde el cual se creó esta conexión. Si una conexión falla durante un intento de actualizar datos, y reconnectionMethod=1, entonces la aplicación de hoja de cálculo volverá a intentarlo usando la información del archivo de conexión externa en lugar del objeto de conexión incrustado en el libro. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Indica si la aplicación de hoja de cálculo debe siempre y solo usar la información de conexión en el archivo de conexión externa indicado por el atributo odcFile cuando se actualiza la conexión. Si false, entonces la aplicación de hoja de cálculo debe seguir el procedimiento indicado por el atributo reconnectionMethod. |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Obtiene [`ConnectionParameterCollection`](../connectionparametercollection/) para una consulta ODBC o web. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula/) { get; } | Obtiene la definición de la fórmula de Power Query. |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Especifica lo que la aplicación de hoja de cálculo debe hacer cuando una conexión falla. El valor predeterminado es ReConnectionMethodType.Required. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Especifica lo que la aplicación de hoja de cálculo debe hacer cuando una conexión falla. El valor predeterminado es ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Especifica el número de minutos entre actualizaciones automáticas de la conexión. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | True si esta conexión debe actualizarse al abrir el archivo; de lo contrario, false. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | True si los datos externos obtenidos a través de la conexión para rellenar una tabla deben guardarse con el libro; de lo contrario, false. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | True si la contraseña debe guardarse como parte de la cadena de conexión; de lo contrario, False. |
| virtual [SecondCommand](../../aspose.cells.externalconnections/externalconnection/secondcommand/) { get; set; } | Especifica una segunda cadena de texto de comando que se conserva cuando se utilizan campos de página basados en servidor de PivotTable. Para conexiones ODBC, serverCommand suele ser una consulta más amplia que command (no hay cláusula WHERE presente en la primera). Basado en estos 2 comandos (Command y ServerCommand), la interfaz de usuario de parámetros puede poblarse y pueden construirse consultas parametrizadas |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Se utiliza cuando la fuente de datos externa es basada en archivos. Cuando una conexión a dicha fuente de datos falla, la aplicación de hoja de cálculo intenta conectarse directamente a este archivo. Puede expresarse en notación URI o ruta de archivo específica del sistema. |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Obtiene o establece el tipo de DataSource de la conexión externa. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Identificador para Single Sign On (SSO) usado para la autenticación entre un servidor intermedio spreadsheetML y la fuente de datos externa. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsolete.**) Obtiene o establece el tipo de DataSource de la conexión externa. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassExternalConnectionDemo
    {
        public static void Run()
        {
            string sourceDir = "Your Source Directory";

            Workbook workbook = new Workbook(sourceDir + "example.xlsx");
            ExternalConnectionCollection conns = workbook.DataConnections;
            foreach (ExternalConnection conn in conns)
            {
                if (conn is DBConnection dbConn)
                {
                    Console.WriteLine("Connection Info: " + dbConn.ConnectionInfo);
                    Console.WriteLine("Formula Definition: " + dbConn.PowerQueryFormula.FormulaDefinition);
                }
            }

            workbook = new Workbook(sourceDir + "example.xlsm");
            conns = workbook.DataConnections;
            foreach (ExternalConnection conn in conns)
            {
                if (conn is DBConnection dbConn)
                {
                    Console.WriteLine("Connection Info: " + dbConn.ConnectionInfo);
                    Console.WriteLine("Formula Definition: " + dbConn.PowerQueryFormula.FormulaDefinition);
                }
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


