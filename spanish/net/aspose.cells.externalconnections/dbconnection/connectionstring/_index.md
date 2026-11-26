---
title: "DBConnection.ConnectionString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DBConnection. La cadena de información de conexión se usa para establecer contacto con una fuente de datos OLE DB o ODBC"
type: docs
url: /es/net/aspose.cells.externalconnections/dbconnection/connectionstring/
---
## DBConnection.ConnectionString property

La cadena de información de conexión se usa para contactar con una fuente de datos OLE DB o ODBC.

```csharp
public override string ConnectionString { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            try
            {
                // Acceder a la colección de conexiones externas
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Crea una nueva DBConnection añadiéndola a la colección
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Muestra el valor inicial de ConnectionString
                Console.WriteLine("Initial ConnectionString: " + dbConnection.ConnectionString);

                // Establece una nueva cadena de conexión
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";

                // Muestra el valor actualizado de ConnectionString
                Console.WriteLine("Updated ConnectionString: " + dbConnection.ConnectionString);

                // Guarda el libro de trabajo
                workbook.Save("ConnectionStringDemo.xlsx");
                Console.WriteLine("ConnectionString demonstration completed successfully.");
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


