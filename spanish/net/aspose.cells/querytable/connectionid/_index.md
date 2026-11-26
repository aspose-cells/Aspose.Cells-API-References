---
title: "QueryTable.ConnectionId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad QueryTable. Obtiene el id de conexión de la tabla de consulta"
type: docs
url: /es/net/aspose.cells/querytable/connectionid/
---
## QueryTable.ConnectionId property

Obtiene el id de conexión de la tabla de consulta.

```csharp
public int ConnectionId { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyConnectionIdDemo
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

                    // Mostrar el valor de la propiedad ConnectionId (solo lectura)
                    Console.WriteLine("Query Table ConnectionId: " + queryTable.ConnectionId);

                    // Mostrar otras propiedades relacionadas para contexto
                    Console.WriteLine("Query Table Name: " + queryTable.Name);
                    Console.WriteLine("External Connection: " +
                        (queryTable.ExternalConnection != null ? queryTable.ExternalConnection.Name : "None"));
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Guarda el libro de trabajo
                workbook.Save("ConnectionIdDemo.xlsx");
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

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


