---
title: "Axis.IsVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis egenskap. Representerar om axeln är synlig"
type: docs
url: /sv/net/aspose.cells.charts/axis/isvisible/
---
## Axis.IsVisible property

Anger om axeln är synlig.

```csharp
public bool IsVisible { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Lägg till en sekundär axelserie
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries[1].PlotOnSecondAxis = true;

            // Demonstrera IsVisible-egenskapen
            Console.WriteLine("Secondary Value Axis Visible: " + chart.SecondValueAxis.IsVisible);
            
            // Dölj den sekundära axeln
            chart.SecondValueAxis.IsVisible = false;
            Console.WriteLine("After setting to false - Secondary Value Axis Visible: " + chart.SecondValueAxis.IsVisible);

            // Spara arbetsboken
            workbook.Save("AxisIsVisibleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


