---
title: "SeriesLayoutProperties.MapLabelLayout"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SeriesLayoutProperties-egenskap. Hämtar och anger layouten för kartetiketter"
type: docs
url: /sv/net/aspose.cells.charts/serieslayoutproperties/maplabellayout/
---
## SeriesLayoutProperties.MapLabelLayout property

Hämtar och anger layouten för kartetiketter.

```csharp
public MapChartLabelLayout MapLabelLayout { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyMapLabelLayoutDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för kartdiagram
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("United States");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["B3"].PutValue(80);
            worksheet.Cells["A4"].PutValue("Mexico");
            worksheet.Cells["B4"].PutValue(60);

            // Lägg till ett kartdiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            Series series = chart.NSeries[0];
            series.XValues = "A2:A4";

            // Konfigurera kartlayoutens egenskaper
            series.LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;
            series.LayoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;
            series.LayoutProperties.MapChartRegionType = MapChartRegionType.DataOnly;

            // Spara arbetsboken
            workbook.Save("MapLabelLayoutDemo.xlsx");
        }
    }
}
```

### Se även

* enum [MapChartLabelLayout](../../mapchartlabellayout/)
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


