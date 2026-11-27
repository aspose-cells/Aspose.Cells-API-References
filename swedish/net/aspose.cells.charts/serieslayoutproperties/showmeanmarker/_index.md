---
title: "SeriesLayoutProperties.ShowMeanMarker"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SeriesLayoutProperties-egenskap. Anger om markörer som visar medelvärdet visas"
type: docs
url: /sv/net/aspose.cells.charts/serieslayoutproperties/showmeanmarker/
---
## SeriesLayoutProperties.ShowMeanMarker property

Anger om markörer som visar medelvärdet visas.

```csharp
public bool ShowMeanMarker { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowMeanMarkerDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Skapa diagram (använd kolumndiagramtyp som stöder medelvärdesmarkörer)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till serie
            chart.NSeries.Add("A1:A4", true);
            Series series = chart.NSeries[0];

            // Konfigurera layoutegenskaper med ShowMeanMarker
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;
            layoutProperties.ShowMeanMarker = true;
            layoutProperties.ShowMeanLine = true;

            // Spara utdata
            workbook.Save("ColumnChartWithMeanMarker.xlsx");
        }
    }
}
```

### Se även

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


