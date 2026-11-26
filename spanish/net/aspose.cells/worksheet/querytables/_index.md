---
title: "Worksheet.QueryTables"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene QueryTableCollection en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/querytables/
---
## Worksheet.QueryTables property

Obtiene [`QueryTableCollection`](../../querytablecollection/) en la hoja de cálculo.

```csharp
public QueryTableCollection QueryTables { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyQueryTablesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            
            // Obtenga la primera tabla de consulta (ya que no podemos agregar nuevas directamente)
            // Nota: la colección QueryTables es de solo lectura en esta versión de la API
            if (worksheet.QueryTables.Count > 0)
            {
                QueryTable queryTable = worksheet.QueryTables[0];
                
                // Mostrar información de la tabla de consulta
                Console.WriteLine("Query Table Name: " + queryTable.Name);
                Console.WriteLine("Result Range: " + queryTable.ResultRange.Address);
                Console.WriteLine("Number of Query Tables: " + worksheet.QueryTables.Count);
            }
            else
            {
                Console.WriteLine("No query tables found in the worksheet.");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("QueryTableDemo.xlsx");
        }
    }
}
```

### Ver también

* class [QueryTableCollection](../../querytablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


