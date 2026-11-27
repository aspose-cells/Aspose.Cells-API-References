---
title: "Enum SparklineType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.SparklineType enum. Representerar sparkline-typerna"
type: docs
url: /sv/net/aspose.cells.charts/sparklinetype/
---
## SparklineType enumeration

Representerar sparkline‑typerna.

```csharp
public enum SparklineType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Line | `0` | Linje-sparkline. |
| Column | `1` | Kolumn-sparkline. |
| Stacked | `2` | Representerar en Vinst/Förlust-sparkline. |
| WinLoss | `2` | Representerar en Vinst/Förlust-sparkline. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineTypeDemo
    {
        public static void SparklineTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Definiera CellArea för sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Lägg till en sparkline‑grupp i kalkylbladet
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];

            // Lägg till sparklines i gruppen
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Anpassa sparkline-gruppen
            CellsColor clr = workbook.CreateCellsColor();
            clr.Color = Color.Orange;
            group.SeriesColor = clr;

            // Ställ in att de höga punkterna färgas gröna och de låga punkterna färgas röda
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            group.HighPointColor.Color = Color.Green;
            group.LowPointColor.Color = Color.Red;

            // Ställ in linjebredd
            group.LineWeight = 1.0;

            // Spara arbetsboken
            workbook.Save("SparklineTypeExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


