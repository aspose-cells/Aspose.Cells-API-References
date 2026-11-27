---
title: "Chart.AutoScaling"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart egenskap. Sant om Microsoft Excel skalar ett 3D-diagram så att det blir närmare i storlek det motsvarande 2D-diagrammet. RightAngleAxes‑egenskapen måste vara True"
type: docs
url: /sv/net/aspose.cells.charts/chart/autoscaling/
---
## Chart.AutoScaling property

Sant om Microsoft Excel skalar ett 3‑D‑diagram så att det är närmare i storlek till motsvarande 2‑D‑diagram. Egenskapen RightAngleAxes måste vara True.

```csharp
public bool AutoScaling { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyAutoScalingDemo
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

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demonstrera AutoScaling‑egenskapen
            chart.AutoScaling = false;
            Console.WriteLine("Chart AutoScaling is set to: " + chart.AutoScaling);

            // Spara arbetsboken
            workbook.Save("ChartAutoScalingDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


