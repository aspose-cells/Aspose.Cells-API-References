---
title: "PlotArea.X"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PlotArea‑egenskap. Hämtar eller sätter x‑koordinaten för det övre vänstra hörnet av plot‑områdets avgränsningsruta i enheter av 1/4000 av diagramområdet."
type: docs
url: /sv/net/aspose.cells.charts/plotarea/x/
---
## PlotArea.X property

Hämtar eller sätter x‑koordinaten för det övre vänstra hörnet av plot‑områdets avgränsningsruta i enheter av 1/4000 av diagramområdet.

```csharp
[Obsolete("Use PlotArea.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```

### Anmärkningar

Plotarea-omslutningsrutan inkluderar plotområdet, stapelmärken (stapelmärkesetiketter) och en liten kant runt stapelmärkena. Om värdet inte skapats av MS Excel, vänligen anropa metoden Chart.Calculate() innan du anropar denna metod.

The **X**, **Y**, **Width** och **Height** för **PlotArea** representerar plot‑områdets avgränsningsruta som inkluderar plotområdet, staplar (stapeltiketter) och en liten kant runt staplarna. Om du vill få den faktiska storleken på plotområdet bör du anropa egenskaperna **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** och **InnerHeightRatioToChart**.

För Excel 2007 eller senare är standardvärdet noll. Du bör hämta värdet efter att ha anropat Chart.Calculate().

Obs: När X sätts kommer egenskapen IsInnerMode automatiskt att sättas till false.

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen PlotArea.XRatioToChart. X = XRatioToChart * 4000. Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyXDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ange PlotArea‑egenskaper
            chart.PlotArea.X = 100;  // Demonstrate X property usage
            chart.PlotArea.Y = 200;
            chart.PlotArea.Width = 1000;
            chart.PlotArea.Height = 800;

            // Spara arbetsboken
            workbook.Save("PlotAreaPropertyXDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


