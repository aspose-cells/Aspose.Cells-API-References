---
title: "Marker.BackgroundColorSetType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Marker-egenskap. Hämtar eller anger typen för markörens bakgrundsfärg"
type: docs
url: /sv/net/aspose.cells.charts/marker/backgroundcolorsettype/
---
## Marker.BackgroundColorSetType property

Hämtar eller anger markörens bakgrundsfärgtyp.

```csharp
public FormattingType BackgroundColorSetType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class MarkerPropertyBackgroundColorSetTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till serie
            int seriesIndex = chart.NSeries.Add("A1:B3", true);
            Series series = chart.NSeries[seriesIndex];

            // Konfigurera markörens egenskaper
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;
            series.Marker.BackgroundColor = System.Drawing.Color.Yellow;

            // Spara arbetsboken
            workbook.Save("MarkerBackgroundColorSetTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [FormattingType](../../formattingtype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


