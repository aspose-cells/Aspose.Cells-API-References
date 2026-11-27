---
title: "Klass AxisBins"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.AxisBins klass. Representerar axis bins"
type: docs
url: /sv/net/aspose.cells.charts/axisbins/
---
## AxisBins class

Representerar axelintervall

```csharp
public class AxisBins
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Count](../../aspose.cells.charts/axisbins/count/) { get; set; } | Hämtar eller anger antalet axis bins |
| [IsAutomatic](../../aspose.cells.charts/axisbins/isautomatic/) { get; set; } | Anger om axis bins är automatiska. |
| [IsByCategory](../../aspose.cells.charts/axisbins/isbycategory/) { get; set; } | Anger om gruppering av data efter kategori är aktiverad. |
| [Overflow](../../aspose.cells.charts/axisbins/overflow/) { get; set; } | Hämtar eller anger overflow för axis bins |
| [Underflow](../../aspose.cells.charts/axisbins/underflow/) { get; set; } | Hämtar eller anger underflow för axis bins |
| [Width](../../aspose.cells.charts/axisbins/width/) { get; set; } | Hämtar eller anger bredden på axis bin. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [ResetOverflow](../../aspose.cells.charts/axisbins/resetoverflow/)() | (**Obsolete.**) Återställ overflow |
| [ResetUnderflow](../../aspose.cells.charts/axisbins/resetunderflow/)() | (**Obsolete.**) Återställ underflow |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisBinsDemo
    {
        public static void AxisBinsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            // Lägg till ett nytt arbetsblad
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till dataserier i diagrammet
            chart.NSeries.Add("A1:A5", true);

            // Åtkomst till värdeaxeln
            Axis valueAxis = chart.ValueAxis;

            // Åtkomst till behållarna på värdeaxeln
            AxisBins bins = valueAxis.Bins;

            // Ställ in egenskaper för behållarna
            bins.IsByCategory = false;
            bins.IsAutomatic = true;
            bins.Width = 10.0;
            bins.Count = 5;
            bins.Overflow = 60.0;
            bins.Underflow = 0.0;

            // Återställ overflow och underflow
            //bins.ResetOverflow();
            //bins.ResetUnderflow();

            // Spara arbetsboken
            workbook.Save("AxisBinsExample.xlsx");
            workbook.Save("AxisBinsExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


