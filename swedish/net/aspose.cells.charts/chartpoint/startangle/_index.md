---
title: "ChartPoint.StartAngle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint egenskap. Hämtar startvinkeln för pajsektionen, mätt i grader medurs från x-axeln efter att ha anropat metoden Chart.Calculate. Gäller för pajdiagram."
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/startangle/
---
## ChartPoint.StartAngle property

Hämtar startvinkeln för pajsektionen, mätt i grader medurs från x-axeln efter att ha anropat metoden Chart.Calculate(). Gäller för pajdiagram.

```csharp
public float StartAngle { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyStartAngleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Lägg till ett pajdiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att säkerställa att egenskaperna är fyllda
            chart.Calculate();

            // Hämta den första diagrampunkten
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa StartAngle‑värdet
            Console.WriteLine("StartAngle of first pie slice: " + point.StartAngle);

            // Obs: StartAngle är skrivskyddad, så vi kan inte sätta den direkt.
            // För att ändra startvinkeln måste vi rotera hela pajdiagrammet.
            chart.NSeries[0].FirstSliceAngle = 90; // Rotate pie chart by 90 degrees

            // Beräkna om för att uppdatera vinklarna.
            chart.Calculate();

            // Visa det nya StartAngle‑värdet efter rotation.
            Console.WriteLine("StartAngle after rotation: " + point.StartAngle);

            // Spara arbetsboken
            workbook.Save("ChartPointPropertyStartAngleDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


