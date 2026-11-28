---
title: "Worksheet.SparklineGroups"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Çalışma sayfasındaki sparkline gruplarını alır"
type: docs
url: /tr/net/aspose.cells/worksheet/sparklinegroups/
---
## Worksheet.SparklineGroups property

Çalışma sayfasındaki sparkline gruplarını alır.

```csharp
public SparklineGroupCollection SparklineGroups { get; }
```

### Örnekler

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

            // Test verilerini doldur
            Cells cells = sheet.Cells;
            for (int i = 0; i < 4; i++)
            {
                for (int j = 0; j < 4; j++)
                {
                    cells[i, j].Value = (i + 1) * (j + 1);
                }
            }

            // Sparkline grubu ekle
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

### Ayrıca Bakınız

* class [SparklineGroupCollection](../../../aspose.cells.charts/sparklinegroupcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


