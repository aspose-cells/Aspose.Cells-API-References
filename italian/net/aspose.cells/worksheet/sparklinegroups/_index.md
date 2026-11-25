---
title: "Worksheet.SparklineGroups"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene i gruppi di sparkline nel foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/sparklinegroups/
---
## Worksheet.SparklineGroups property

Ottiene i gruppi di sparkline nel foglio di lavoro.

```csharp
public SparklineGroupCollection SparklineGroups { get; }
```

### Esempi

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

            // Popola dati di test
            Cells cells = sheet.Cells;
            for (int i = 0; i < 4; i++)
            {
                for (int j = 0; j < 4; j++)
                {
                    cells[i, j].Value = (i + 1) * (j + 1);
                }
            }

            // Aggiungi gruppo di sparkline
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

### Vedi anche

* class [SparklineGroupCollection](../../../aspose.cells.charts/sparklinegroupcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


