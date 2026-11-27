---
title: "ChartFrame.DefaultYRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame‑egenskap. Representerar y för standardposition i enheter av bråkdelen av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/defaultyratiotochart/
---
## ChartFrame.DefaultYRatioToChart property

Representerar y för standardpositionen i enheter av en bråkdel av diagramområdet.

```csharp
public double DefaultYRatioToChart { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultYRatioToChartDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
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
            
            // Lägg till ett diagram och hämta dess diagramram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);
            
            // Hämta diagramramen (titel i detta fall)
            ChartFrame chartFrame = chart.Title;
            
            // Visa det aktuella DefaultYRatioToChart‑värdet
            Console.WriteLine("Current DefaultYRatioToChart value: " + chartFrame.DefaultYRatioToChart);
            
            // Demonstrera hur förändring av YRatioToChart påverkar positionen (eftersom DefaultYRatioToChart är skrivskyddad)
            Console.WriteLine("Current YRatioToChart value: " + chartFrame.YRatioToChart);
            chartFrame.YRatioToChart = 0.1; // Move title up
            Console.WriteLine("New YRatioToChart value: " + chartFrame.YRatioToChart);
            
            // Spara resultatet
            workbook.Save("PropertyDefaultYRatioToChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


