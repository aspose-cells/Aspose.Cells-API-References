---
title: "QueryTable.ExternalConnection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad QueryTable. Obtiene la conexión externa relacionada"
type: docs
url: /es/net/aspose.cells/querytable/externalconnection/
---
## QueryTable.ExternalConnection property

Obtiene la conexión externa relacionada.

```csharp
public ExternalConnection ExternalConnection { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class QueryTablePropertyExternalConnectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para simular un escenario de tabla de consulta
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Sample Data");

            try
            {
                // Verifique si hay tablas de consulta en la hoja de cálculo
                if (worksheet.QueryTables.Count > 0)
                {
                    // Obtenga la primera tabla de consulta
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Acceder a la propiedad ExternalConnection (solo lectura)
                    ExternalConnection externalConnection = queryTable.ExternalConnection;

                    // Mostrar información sobre la conexión externa
                    if (externalConnection != null)
                    {
                        Console.WriteLine("External Connection ID: " + externalConnection.Id);
                        Console.WriteLine("External Connection Name: " + externalConnection.Name);
                        Console.WriteLine("External Connection Type: " + externalConnection.ClassType);
                        Console.WriteLine("Connection String: " + externalConnection.ConnectionString);
                        Console.WriteLine("Refresh on Load: " + externalConnection.RefreshOnLoad);
                    }
                    else
                    {
                        Console.WriteLine("No external connection associated with this query table.");
                    }

                    // Mostrar otras propiedades de la tabla de consulta para contexto
                    Console.WriteLine("Query Table Name: " + queryTable.Name);
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Guarda el libro de trabajo
                workbook.Save("ExternalConnectionDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


