---
title: "ChartFrame.X"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame‑egenskap. Hämtar eller anger x‑koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/x/
---
## ChartFrame.X property

Hämtar eller anger x‑koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet.

```csharp
[Obsolete("Use ChartFrame.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int X { get; set; }
```

### Anmärkningar

Hur konverterar man enheter av 1/4000 till pixlar? X i pixlar = X * Chart.ChartObject.Width / 4000d;

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.XRatioToChart. X = XRatioToChart * 4000. Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyXDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("X Values");
            sheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
            }

            // Lägg till diagram
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Lägg till serier och ange X/Y‑värden
            chart.NSeries.Add("Sheet1!B2:B10", true);
            chart.NSeries[0].XValues = "Sheet1!A2:A10";

            // Lägg till trendlinje
            chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "Linear Trend");
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            
            // Konfigurera datamärkningar
            trendline.DataLabels.ShowValue = true;
            trendline.DataLabels.Font.Color = Color.Blue;
            
            // Demonstrera användning av X‑egenskapen
            trendline.DataLabels.X = -500; // Set X position offset
            trendline.DataLabels.Y = 200;  // Set Y position offset

            // Spara arbetsboken
            workbook.Save("ChartFramePropertyXDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


