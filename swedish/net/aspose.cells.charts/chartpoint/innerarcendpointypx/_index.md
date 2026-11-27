---
title: "ChartPoint.InnerArcEndPointYPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar y-koordinaten för slutpunkten för pajsektionen efter anrop av metoden Chart.Calculate. Gäller för donut-diagram."
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/innerarcendpointypx/
---
## ChartPoint.InnerArcEndPointYPx property

Hämtar y-koordinaten för slutpunkten för pajsektionen efter att anropa metoden Chart.Calculate(). Gäller för Doughnut-diagram.

```csharp
public float InnerArcEndPointYPx { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcEndPointYPxDemo
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
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["B3"].PutValue(35);
            worksheet.Cells["B4"].PutValue(25);

            // Lägg till ett doughnut-diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att få diagrampunkts-egenskaperna
            chart.Calculate();

            // Hämta den första diagrampunkten från den första serien
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa det aktuella InnerArcEndPointYPx-värdet
            Console.WriteLine("Current InnerArcEndPointYPx value: " + point.InnerArcEndPointYPx);

            // Obs: InnerArcEndPointYPx är skrivskyddad, så vi kan inte sätta den direkt
            // För att ändra positionen måste vi ändra storleken på donut-hålet
            chart.NSeries[0].DoughnutHoleSize = 60; // Change hole size to affect inner arc position

            // Beräkna om diagrammet för att uppdatera egenskaperna
            chart.Calculate();

            // Visa det nya InnerArcEndPointYPx-värdet efter att hålstorleken har ändrats
            Console.WriteLine("New InnerArcEndPointYPx value after changing hole size: " + point.InnerArcEndPointYPx);

            // Spara arbetsboken
            workbook.Save("ChartPointPropertyInnerArcEndPointYPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


