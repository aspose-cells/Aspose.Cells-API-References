---
title: "Enum SparklineAxisMinMaxType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.SparklineAxisMinMaxType enum. Representerar minsta och största värdetyperna för sparkline-vertikalaxeln"
type: docs
url: /sv/net/aspose.cells.charts/sparklineaxisminmaxtype/
---
## SparklineAxisMinMaxType enumeration

Representerar minsta och största värdetyper för sparkline‑vertikalaxeln.

```csharp
public enum SparklineAxisMinMaxType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| AutoIndividual | `0` | Automatiskt för varje sparkline. |
| Group | `1` | Samma för alla sparklines i gruppen. |
| Custom | `2` | Anpassat värde för sparkline. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineAxisMinMaxTypeDemo
    {
        public static void SparklineAxisMinMaxTypeExample()
        {
            // Skapa en arbetsbok och ett kalkylblad
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Definiera CellArea
            CellArea cellArea = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Lägg till en sparkline‑grupp i kalkylbladet
            int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];
            sparklineGroup.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Ange egenskaper för sparkline-gruppen
            sparklineGroup.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Group;
            sparklineGroup.VerticalAxisMinValueType = SparklineAxisMinMaxType.AutoIndividual;

            // Skapa CellsColor
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = Color.Green;
            sparklineGroup.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = Color.Red;
            sparklineGroup.LowPointColor = lowPointColor;

            // Ange ytterligare egenskaper
            sparklineGroup.ShowHighPoint = true;
            sparklineGroup.ShowLowPoint = true;
            sparklineGroup.LineWeight = 1.0;

            // Spara arbetsboken
            workbook.Save("SparklineAxisMinMaxTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


