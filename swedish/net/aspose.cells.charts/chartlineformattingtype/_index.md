---
title: "Enum ChartLineFormattingType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.ChartLineFormattingType enum. Representerar linjeformattyp för diagramlinjen"
type: docs
url: /sv/net/aspose.cells.charts/chartlineformattingtype/
---
## ChartLineFormattingType enumeration

Representerar linjeformattypen för diagramlinjen.

```csharp
public enum ChartLineFormattingType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Automatic | `0` | Representerar automatisk formateringstyp. |
| Solid | `1` | Representerar solid formateringstyp. |
| None | `2` | Representerar ingen formateringstyp. |
| Gradient | `3` | Gradient |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartLineFormattingTypeDemo
    {
        public static void ChartLineFormattingTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till serier i diagrammet
            chart.NSeries.Add("A1:B3", true);
            
            // Ange kategoridata
            chart.NSeries.CategoryData = "A1:A3";
            
            // Ange olika linjeformateringstyper för serien
            chart.NSeries[0].SeriesLines.FormattingType = ChartLineFormattingType.Solid;
            chart.NSeries[0].SeriesLines.Color = Color.Red;
            
            // Lägg till en annan serie med annan formatering
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries[1].SeriesLines.FormattingType = ChartLineFormattingType.Gradient;
            chart.NSeries[1].SeriesLines.Color = Color.Blue;
            
            // Spara arbetsboken
            workbook.Save("ChartLineFormattingTypeExample.xlsx");
            workbook.Save("ChartLineFormattingTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


