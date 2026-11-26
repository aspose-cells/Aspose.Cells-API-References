---
title: "Worksheet.Filter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Filtra el rango"
type: docs
url: /es/net/aspose.cells/worksheet/filter/
---
## Worksheet.Filter method

Filtra el rango.

```csharp
public void Filter(CellArea ca)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | CellArea | El rango |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class WorksheetMethodFilterWithCellAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellena algunos datos de ejemplo (incluyendo una fila de encabezado)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            try
            {
                // Defina el rango al que se aplicará el filtro
                CellArea filterArea = new CellArea
                {
                    StartRow = 0,      // Row 1 (zero‑based)
                    StartColumn = 0,   // Column A
                    EndRow = 4,        // Row 5
                    EndColumn = 1      // Column B
                };

                // Aplique un autofiltro al área definida
                worksheet.Filter(filterArea);

                // Guarde el libro de trabajo para verificar que el filtro se haya establecido
                workbook.Save("WorksheetFilterWithCellAreaDemo.xlsx");

                Console.WriteLine("Filter applied successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error applying filter: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


