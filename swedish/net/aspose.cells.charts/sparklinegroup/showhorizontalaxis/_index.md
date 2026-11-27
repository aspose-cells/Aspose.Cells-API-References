---
title: "SparklineGroup.ShowHorizontalAxis"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup-egenskap. Anger om den horisontella axeln för sparkline ska visas. Den horisontella axeln visas om sparkline har data som korsar nollaxeln."
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/showhorizontalaxis/
---
## SparklineGroup.ShowHorizontalAxis property

Anger om den horisontella axeln för sparkline ska visas. Den horisontella axeln visas om sparkline har data som korsar nollaxeln.

```csharp
public bool ShowHorizontalAxis { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowHorizontalAxisDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Definiera sparkline-plats
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

            // Konfigurera sparkline-egenskaper
            group.ShowHorizontalAxis = true;
            CellsColor axisColor = workbook.CreateCellsColor();
            axisColor.Color = Color.Gray;
            group.HorizontalAxisColor = axisColor;

            // Spara arbetsboken
            workbook.Save("SparklineWithHorizontalAxis.xlsx");
        }
    }
}
```

### Se även

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


