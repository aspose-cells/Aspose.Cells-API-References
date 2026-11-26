---
title: "QueryTable.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad QueryTable. Obtiene el nombre de la tabla de consulta"
type: docs
url: /es/net/aspose.cells/querytable/name/
---
## QueryTable.Name property

Obtiene el nombre de la querytable.

```csharp
public string Name { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para simular una tabla de consulta
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            try
            {
                // Verifique si hay tablas de consulta en la hoja de cálculo
                if (worksheet.QueryTables.Count > 0)
                {
                    // Obtenga la primera tabla de consulta
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Mostrar el valor de la propiedad Name (operación de solo lectura)
                    Console.WriteLine("Query Table Name: " + queryTable.Name);

                    // Mostrar otras propiedades de solo lectura para contexto
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                    Console.WriteLine("Result Range: " + queryTable.ResultRange.Address);
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Guarda el libro de trabajo
                workbook.Save("QueryTableNameDemo.xlsx");
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


