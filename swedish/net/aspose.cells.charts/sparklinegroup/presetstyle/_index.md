---
title: "SparklineGroup.PresetStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup-egenskap. Hämtar och anger den förinställda stiltypen för sparkline-gruppen"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/presetstyle/
---
## SparklineGroup.PresetStyle property

Hämtar och anger den förinställda stiltypen för sparkline-gruppen.

```csharp
public SparklinePresetStyleType PresetStyle { get; set; }
```

### Anmärkningar

Om den här egenskapen är inställd, kommer dessa egenskaper: SeriesColor,NegativePointsColor,HorizontalAxisColor,MarkersColor,FirstPointColor,LastPointColor,HighPointColor,LowPointColor att täckas. Så vänligen ange egenskapen först, sedan ange de andra.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyPresetStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempeldata
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(3);
            worksheet.Cells["C1"].PutValue(7);
            worksheet.Cells["D1"].PutValue(2);
            worksheet.Cells["E1"].PutValue(9);

            // Skapa sparkline-grupp
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 5;
            ca.EndColumn = 5;
            int index = worksheet.SparklineGroups.Add(SparklineType.Column, "A1:E1", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[index];

            // Applicera förinställd stil
            group.PresetStyle = SparklinePresetStyleType.Style5;

            workbook.Save("SparklinePresetStyleDemo.xlsx");
        }
    }
}
```

### Se även

* enum [SparklinePresetStyleType](../../sparklinepresetstyletype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


