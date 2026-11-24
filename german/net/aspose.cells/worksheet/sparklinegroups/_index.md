---
title: "Worksheet.SparklineGroups"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt die Sparkline-Gruppen im Arbeitsblatt zurück"
type: docs
url: /de/net/aspose.cells/worksheet/sparklinegroups/
---
## Worksheet.SparklineGroups property

Ruft die Sparkline‑Gruppen im Arbeitsblatt ab.

```csharp
public SparklineGroupCollection SparklineGroups { get; }
```

### Beispiele

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

            // Fülle Testdaten
            Cells cells = sheet.Cells;
            for (int i = 0; i < 4; i++)
            {
                for (int j = 0; j < 4; j++)
                {
                    cells[i, j].Value = (i + 1) * (j + 1);
                }
            }

            // Sparkline-Gruppe hinzufügen
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

### Siehe auch

* class [SparklineGroupCollection](../../../aspose.cells.charts/sparklinegroupcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


