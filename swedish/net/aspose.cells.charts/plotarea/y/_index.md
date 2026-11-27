---
title: "PlotArea.Y"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PlotArea-egenskap. Hämtar eller anger y-koordinaten för den övre hörnet av plotarea-omslutningsrutan i enheter av 1/4000 av diagramområdet."
type: docs
url: /sv/net/aspose.cells.charts/plotarea/y/
---
## PlotArea.Y property

Hämtar eller anger y-koordinaten för den övre hörnet av plotarea-omslutningsrutan i enheter av 1/4000 av diagramområdet.

```csharp
[Obsolete("Use PlotArea.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```

### Anmärkningar

Plotarea-omslutningsrutan inkluderar plotområdet, stapelmärken (stapelmärkesetiketter) och en liten kant runt stapelmärkena. Om värdet inte skapats av MS Excel, vänligen anropa metoden Chart.Calculate() innan du anropar denna metod.

The **X**, **Y**, **Width** och **Height** för **PlotArea** representerar plot‑områdets avgränsningsruta som inkluderar plotområdet, staplar (stapeltiketter) och en liten kant runt staplarna. Om du vill få den faktiska storleken på plotområdet bör du anropa egenskaperna **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** och **InnerHeightRatioToChart**.

För Excel 2007 eller senare är standardvärdet noll. Du bör hämta värdet efter att ha anropat Chart.Calculate().

Obs: När Y sätts kommer egenskapen IsInnerMode automatiskt att sättas till false.

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen PlotArea.YRatioToChart. Y = YRatioToChart * 4000. Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Exempeldata
            sheet.Cells["A1"].PutValue("Category 1");
            sheet.Cells["A2"].PutValue("Category 2");
            sheet.Cells["B1"].PutValue(100);
            sheet.Cells["B2"].PutValue(50);

            // Skapa diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Ange diagramdata
            chart.NSeries.Add("B1:B2", false);
            chart.NSeries.CategoryData = "A1:A2";

            // Konfigurera plot-området
            chart.PlotArea.Width = 300;
            chart.PlotArea.Height = 200;
            chart.PlotArea.X = 100;
            chart.PlotArea.Y = 150; // Demonstrating Y property usage

            // Spara arbetsboken
            workbook.Save("PlotAreaPropertyYDemo.xlsx");
        }
    }
}
```

### Se även

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


