---
title: "Workbook.DataMashup"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Workbook. Obtiene los datos de mashup"
type: docs
url: /es/net/aspose.cells/workbook/datamashup/
---
## Workbook.DataMashup property

Obtiene los datos mashup.

```csharp
public DataMashup DataMashup { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDataMashupDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para activar Power Query
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(150);

            // Guardar en un archivo
            string sourcePath = "source.xlsx";
            workbook.Save(sourcePath);

            // Reabrir el libro de trabajo para acceder a DataMashup
            workbook = new Workbook(sourcePath);
            
            // Acceder a las fórmulas de Power Query a través de la propiedad DataMashup
            var queries = workbook.DataMashup.PowerQueryFormulas;
            
            // Mostrar información básica sobre las consultas
            Console.WriteLine($"Number of Power Query formulas: {queries.Count}");
            
            // Si hay consultas, mostrar los detalles de la primera
            if (queries.Count > 0)
            {
                foreach (var query in queries)
                {
                    Console.WriteLine($"Query Name: {query.Name}");
                    Console.WriteLine($"Number of items: {query.PowerQueryFormulaItems.Count}");
                    break; // Just show first query for demo
                }
            }

            // Guardar en un archivo nuevo
            string destPath = "output.xlsx";
            workbook.Save(destPath);
        }
    }
}
```

### Ver también

* class [DataMashup](../../../aspose.cells.querytables/datamashup/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


