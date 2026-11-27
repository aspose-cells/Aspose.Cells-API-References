---
title: "SparklineGroup.NegativePointsColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup egenskap. Hämtar och anger färgen på de negativa värdena i sparkline-gruppen"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/negativepointscolor/
---
## SparklineGroup.NegativePointsColor property

Hämtar och anger färgen på de negativa värdena i sparkline-gruppen.

```csharp
public CellsColor NegativePointsColor { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyNegativePointsColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till data med negativa värden för att demonstrera negativa punkter
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

            // Lägg till sparkline-grupp
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Konfigurera färg för negativa punkter
            group.ShowNegativePoints = true;
            CellsColor negativePointsColor = workbook.CreateCellsColor();
            negativePointsColor.Color = Color.Blue;
            group.NegativePointsColor = negativePointsColor;

            workbook.Save("SparklineNegativePointsColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


