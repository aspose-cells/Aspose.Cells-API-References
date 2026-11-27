---
title: "SparklineGroup.Sparklines"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup egenskap. Hämtar samlingen av Sparkline-objekt"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/sparklines/
---
## SparklineGroup.Sparklines property

Hämtar samlingen av [`Sparkline`](../../sparkline/) objekt.

```csharp
public SparklineCollection Sparklines { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertySparklinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Skapa sparkline-grupp
            CellArea location = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 4, EndColumn = 4 };
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, location);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Lägg till sparkline med hjälp av egenskapen Sparklines
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Anpassa sparkline-utseende
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;

            // Spara arbetsboken
            workbook.Save("SparklineDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [SparklineCollection](../../sparklinecollection/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


