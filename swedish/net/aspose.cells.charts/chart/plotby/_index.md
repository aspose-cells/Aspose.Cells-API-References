---
title: "Chart.PlotBy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagramegenskap. Hämtar och anger om plottning sker per rad eller kolumn"
type: docs
url: /sv/net/aspose.cells.charts/chart/plotby/
---
## Chart.PlotBy property

Hämtar och anger om plotten ska göras per rad eller kolumn.

```csharp
public PlotDataByType PlotBy { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotByDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.SetChartDataRange("A1:C4", true);

            // Visa PlotBy-egenskapen
            Console.WriteLine("Default PlotBy: " + chart.PlotBy);
            
            // Skapa ett nytt diagram med annan plot by-inställning
            int newChartIndex = worksheet.Charts.Add(ChartType.Column, 25, 0, 40, 8);
            Aspose.Cells.Charts.Chart newChart = worksheet.Charts[newChartIndex];
            newChart.SetChartDataRange("A1:C4", false); // Plot by row
            Console.WriteLine("New chart PlotBy: " + newChart.PlotBy);

            // Spara arbetsboken
            workbook.Save("ChartPropertyPlotByDemo_out.xlsx");
        }
    }
}
```

### Se även

* enum [PlotDataByType](../../plotdatabytype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


