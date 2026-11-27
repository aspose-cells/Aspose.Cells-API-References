---
title: "PlotArea.InnerHeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PlotArea-egenskap. Hämtar eller anger höjden på plotområdet i enheter av 1/4000 av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/plotarea/innerheight/
---
## PlotArea.InnerHeight property

Hämtar eller anger höjden på plotområdet i enheter av 1/4000 av diagramområdet.

```csharp
[Obsolete("Use PlotArea.InnerHeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerHeight { get; set; }
```

### Anmärkningar

Plotarea-omslutningsrutan inkluderar plotområdet, stapelmärken (stapelmärkesetiketter) och en liten kant runt stapelmärkena. Om värdet inte skapats av MS Excel, vänligen anropa metoden Chart.Calculate() innan du anropar denna metod.

The **X**, **Y**, **Width** och **Height** för **PlotArea** representerar plot‑områdets avgränsningsruta som inkluderar plotområdet, staplar (stapeltiketter) och en liten kant runt staplarna. Om du vill få den faktiska storleken på plotområdet bör du anropa egenskaperna **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** och **InnerHeightRatioToChart**.

För Excel 2007 eller senare är standardvärdet noll. Du bör hämta värdet efter att ha anropat Chart.Calculate().

Obs: När InnerHeight anges, kommer egenskapen IsInnerMode automatiskt att sättas till True.

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen PlotArea.InnerHeightRatioToChart. InnerHeight = InnerHeightRatioToChart * 4000; Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyInnerHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagramdata
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Konfigurera plot-området
            PlotArea plotArea = chart.PlotArea;
            plotArea.InnerHeight = 1800; // Demonstrate InnerHeight property
            plotArea.InnerWidth = 2800;
            plotArea.IsInnerMode = true;

            workbook.Save("PlotAreaInnerHeightDemo.xlsx");
        }
    }
}
```

### Se även

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


