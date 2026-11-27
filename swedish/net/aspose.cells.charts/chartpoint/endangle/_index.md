---
title: "ChartPoint.EndAngle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar slutvinkeln för pajavsnittet, mätt i grader medurs från x-axeln efter anrop av metoden Chart.Calculate. Gäller för pajdiagram."
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/endangle/
---
## ChartPoint.EndAngle property

Hämtar slutvinkeln för pajsektionen, mätt i grader medurs från x‑axeln efter att anropa metoden Chart.Calculate(). Gäller för Pie-diagram.

```csharp
public float EndAngle { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyEndAngleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pajdiagram
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Lägg till ett pajdiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att säkerställa att egenskaperna är fyllda
            chart.Calculate();

            // Hämta den första diagrampunkten (äppelskiva)
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa det aktuella värdet för EndAngle
            Console.WriteLine("Current EndAngle value: " + point.EndAngle);

            // Obs: EndAngle är skrivskyddad, så vi kan inte sätta den direkt
            // Istället demonstrerar vi hur den relaterar till pajskivan

            // Explodera punkten för att se hur den påverkar vinklarna
            point.Explosion = 20;
            chart.Calculate(); // Recalculate to update angles

            // Visa det nya värdet för EndAngle efter explosion
            Console.WriteLine("EndAngle after explosion: " + point.EndAngle);

            // Spara arbetsboken
            workbook.Save("ChartPointEndAngleDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


