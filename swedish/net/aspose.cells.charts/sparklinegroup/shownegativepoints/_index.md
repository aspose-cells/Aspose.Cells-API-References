---
title: "SparklineGroup.ShowNegativePoints"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup-egenskap. Anger om de negativa värdena i sparkline-gruppen ska markeras med en annan färg eller markör"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/shownegativepoints/
---
## SparklineGroup.ShowNegativePoints property

Anger om de negativa värdena i sparkline-gruppen ska markeras med en annan färg eller markör.

```csharp
public bool ShowNegativePoints { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowNegativePointsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till data med negativa värden för att demonstrera ShowNegativePoints
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(-2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(-3);

            // Definiera CellArea för sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Lägg till en sparkline-grupp
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Konfigurera sparkline-gruppens egenskaper
            group.ShowNegativePoints = true;
            CellsColor negativePointsColor = workbook.CreateCellsColor();
            negativePointsColor.Color = Color.Blue;
            group.NegativePointsColor = negativePointsColor;

            // Spara arbetsboken
            workbook.Save("SparklineNegativePointsDemo.xlsx");
        }
    }
}
```

### Se även

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


