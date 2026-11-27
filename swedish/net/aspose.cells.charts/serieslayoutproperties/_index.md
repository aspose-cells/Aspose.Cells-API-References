---
title: "Klass SeriesLayoutProperties"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.SeriesLayoutProperties-klass. Representerar egenskaperna för serielayout"
type: docs
url: /sv/net/aspose.cells.charts/serieslayoutproperties/
---
## SeriesLayoutProperties class

Representerar egenskaperna för serielayouten.

```csharp
public class SeriesLayoutProperties
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [SeriesLayoutProperties](serieslayoutproperties/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [IsIntervalLeftClosed](../../aspose.cells.charts/serieslayoutproperties/isintervalleftclosed/) { get; set; } | Anger om intervallet är stängt på vänster sida. |
| [MapChartProjectionType](../../aspose.cells.charts/serieslayoutproperties/mapchartprojectiontype/) { get; set; } | Hämtar och anger projektionstypen för kartan. |
| [MapChartRegionType](../../aspose.cells.charts/serieslayoutproperties/mapchartregiontype/) { get; set; } | Hämtar och anger regionstypen för kartan. |
| [MapLabelLayout](../../aspose.cells.charts/serieslayoutproperties/maplabellayout/) { get; set; } | Hämtar och anger layouten för kartetiketter. |
| [QuartileCalculation](../../aspose.cells.charts/serieslayoutproperties/quartilecalculation/) { get; set; } | Representerar de statistiska egenskaperna för serien. |
| [ShowConnectorLines](../../aspose.cells.charts/serieslayoutproperties/showconnectorlines/) { get; set; } | Anger om anslutningslinjer visas mellan datapunkter. |
| [ShowInnerPoints](../../aspose.cells.charts/serieslayoutproperties/showinnerpoints/) { get; set; } | Anger om icke-utliggare datapunkter ska visas. |
| [ShowMeanLine](../../aspose.cells.charts/serieslayoutproperties/showmeanline/) { get; set; } | Anger om linjen som förbinder alla medelvärdespunkter ska visas. |
| [ShowMeanMarker](../../aspose.cells.charts/serieslayoutproperties/showmeanmarker/) { get; set; } | Anger om markörer som visar medelvärdet visas. |
| [ShowOutlierPoints](../../aspose.cells.charts/serieslayoutproperties/showoutlierpoints/) { get; set; } | Anger om utliggare datapunkter visas. |
| [Subtotals](../../aspose.cells.charts/serieslayoutproperties/subtotals/) { get; set; } | Representerar indexet för en delsumme-datapunkt. |

### Anmärkningar

Gäller endast för BoxWhisker,Funnel,ParetoLine,Sunburst,Treemap,Waterfall och Histogram-diagram.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesLayoutPropertiesDemo
    {
        public static void SeriesLayoutPropertiesExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till serier i diagrammet
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";
            Series series = chart.NSeries[seriesIndex];

            // Ange värdena för serien
            series.Values = "=B1:B4";

            // Åtkomst till SeriesLayoutProperties-objektet
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;

            // Ange egenskaper för SeriesLayoutProperties
            layoutProperties.ShowConnectorLines = true;
            layoutProperties.ShowMeanLine = true;
            layoutProperties.ShowOutlierPoints = true;
            layoutProperties.ShowMeanMarker = true;
            layoutProperties.ShowInnerPoints = true;
            layoutProperties.QuartileCalculation = QuartileCalculationType.Inclusive;
            layoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;
            layoutProperties.IsIntervalLeftClosed = true;
            layoutProperties.MapChartRegionType = MapChartRegionType.World;
            layoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;

            // Spara arbetsboken
            workbook.Save("SeriesLayoutPropertiesExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


