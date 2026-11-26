---
title: "DBConnection.ConnectionInfo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DBConnection. La cadena de información de conexión se usa para establecer contacto con una fuente de datos OLE DB o ODBC"
type: docs
url: /es/net/aspose.cells.externalconnections/dbconnection/connectioninfo/
---
## DBConnection.ConnectionInfo property

La cadena de información de conexión se usa para contactar con una fuente de datos OLE DB o ODBC.

```csharp
[Obsolete("Use ExternalConnection.ConnectionString property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string ConnectionInfo { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ExternalConnection.ConnectionString. Este método será eliminado 12 meses después, a partir de octubre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyConnectionInfoDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            try
            {
                // Crea una nueva instancia de DBConnection añadiéndola a la colección
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Configura una conexión básica para demostrar la propiedad ConnectionInfo
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";

                // Muestra el valor actual de la propiedad ConnectionInfo
                Console.WriteLine("Current ConnectionInfo value: " + dbConnection.ConnectionInfo);

                // Dado que ConnectionInfo no es de solo lectura, demuestra cómo configurarla
                dbConnection.ConnectionInfo = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=D:\\data\\database.mdb;";
                Console.WriteLine("Updated ConnectionInfo value: " + dbConnection.ConnectionInfo);

                // Guarda el libro de trabajo
                workbook.Save("ConnectionInfoDemo.xlsx");

                Console.WriteLine("ConnectionInfo demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


