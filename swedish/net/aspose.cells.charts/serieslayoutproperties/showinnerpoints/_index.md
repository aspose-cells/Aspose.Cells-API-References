---
title: "SeriesLayoutProperties.ShowInnerPoints"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SeriesLayoutProperties egenskap. Anger om icke‑avvikande datapunkter ska visas"
type: docs
url: /sv/net/aspose.cells.charts/serieslayoutproperties/showinnerpoints/
---
## SeriesLayoutProperties.ShowInnerPoints property

Anger om icke-utliggare datapunkter ska visas.

```csharp
public bool ShowInnerPoints { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowInnerPointsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för låddiagram
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(40);
            worksheet.Cells["A4"].PutValue(15);
            worksheet.Cells["A5"].PutValue(20);
            worksheet.Cells["A6"].PutValue(25);
            worksheet.Cells["A7"].PutValue(30);
            worksheet.Cells["A8"].PutValue(35);
            worksheet.Cells["A9"].PutValue(40);
            worksheet.Cells["A10"].PutValue(45);
            worksheet.Cells["A11"].PutValue(50);

            // Lägg till ett låddiagram
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till serier i diagrammet
            chart.NSeries.Add("A2:A11", true);
            Series series = chart.NSeries[0];

            // Ställ in egenskaper för serielayout
            SeriesLayoutProperties layout = series.LayoutProperties;
            layout.ShowInnerPoints = true; // Demonstrate ShowInnerPoints property
            layout.ShowOutlierPoints = true;
            layout.ShowMeanMarker = true;

            // Beräkna diagrammet
            chart.Calculate();

            // Spara arbetsboken
            workbook.Save("BoxWhiskerChart_ShowInnerPoints.xlsx");
        }
    }
}
```

### Se även

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


