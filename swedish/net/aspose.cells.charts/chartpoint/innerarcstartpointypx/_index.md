---
title: "ChartPoint.InnerArcStartPointYPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar y-koordinaten för startpunkten för pajsektionen efter anrop av metoden Chart.Calculate. Gäller för donut-diagram."
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/innerarcstartpointypx/
---
## ChartPoint.InnerArcStartPointYPx property

Hämtar y-koordinaten för startpunkten för pajsektionen efter att anropa metoden Chart.Calculate(). Gäller för Doughnut-diagram.

```csharp
public float InnerArcStartPointYPx { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcStartPointYPxDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("C1");
            worksheet.Cells["A3"].PutValue("C2");
            worksheet.Cells["A4"].PutValue("C3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(2);

            // Lägg till ett doughnut-diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att säkerställa att egenskaperna är fyllda
            chart.Calculate();

            // Hämta den första diagrampunkten
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa InnerArcStartPointYPx-värdet
            Console.WriteLine("InnerArcStartPointYPx: " + point.InnerArcStartPointYPx);

            // Obs: InnerArcStartPointYPx är skrivskyddad, så vi kan inte sätta den direkt
            // För att ändra positionen måste vi justera storleken på donut-hålet
            chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size

            // Beräkna om diagrammet för att uppdatera egenskaperna
            chart.Calculate();

            // Visa det nya InnerArcStartPointYPx-värdet efter att hålstorleken har ändrats
            Console.WriteLine("New InnerArcStartPointYPx after changing hole size: " + point.InnerArcStartPointYPx);

            // Spara arbetsboken
            workbook.Save("ChartPointPropertyInnerArcStartPointYPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


