---
title: "ChartPoint.InnerArcEndPointXPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar x-koordinaten för slutpunkten för pajsektionen efter att ha anropat metoden Chart.Calculate. Gäller för Doughnut-diagram."
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/innerarcendpointxpx/
---
## ChartPoint.InnerArcEndPointXPx property

Hämtar x-koordinaten för slutpunkten för pajsektionen efter att ha anropat metoden Chart.Calculate(). Gäller för Doughnut-diagram.

```csharp
public float InnerArcEndPointXPx { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcEndPointXPxDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att få diagrampunkts-egenskaperna
            chart.Calculate();

            // Hämta den första diagrampunkten från den första serien
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa det aktuella InnerArcEndPointXPx-värdet
            Console.WriteLine("Current InnerArcEndPointXPx value: " + point.InnerArcEndPointXPx);

            // Obs: InnerArcEndPointXPx är skrivskyddad, så vi kan inte sätta den direkt
            // För att ändra slutpunktens position måste vi ändra storleken på doughnut-hålet
            chart.NSeries[0].DoughnutHoleSize = 50; // Set hole size to 50%

            // Beräkna om diagrammet för att uppdatera egenskaperna
            chart.Calculate();

            // Visa det nya InnerArcEndPointXPx-värdet efter att ha ändrat hålets storlek
            Console.WriteLine("New InnerArcEndPointXPx value after changing doughnut hole size: " + point.InnerArcEndPointXPx);

            // Spara arbetsboken
            workbook.Save("ChartPointPropertyInnerArcEndPointXPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


