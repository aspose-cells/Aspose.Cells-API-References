---
title: "Worksheet.SparklineGroups"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene los grupos de sparklines en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/sparklinegroups/
---
## Worksheet.SparklineGroups property

Obtiene los grupos de sparkline en la hoja de cálculo.

```csharp
public SparklineGroupCollection SparklineGroups { get; }
```

### Ejemplos

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertySparklineGroupsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Poblar datos de prueba
            Cells cells = sheet.Cells;
            for (int i = 0; i < 4; i++)
            {
                for (int j = 0; j < 4; j++)
                {
                    cells[i, j].Value = (i + 1) * (j + 1);
                }
            }

            // Agregar grupo de sparkline
            int groupIndex = sheet.SparklineGroups.Add(
                0, // Line sparkline type code
                "A1:D4", 
                false, 
                CellArea.CreateCellArea("F1", "F4")
            );

            workbook.Save("output_sparklines.xlsx");
        }
    }
}
```

### Ver también

* class [SparklineGroupCollection](../../../aspose.cells.charts/sparklinegroupcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


