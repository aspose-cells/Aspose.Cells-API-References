---
title: "ChartPoint.ArcStartPointXPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar x-koordinaten för startpunkten för pajavsnittet efter att ha anropat metoden Chart.Calculate. Gäller för paj- och munkdiagram."
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/arcstartpointxpx/
---
## ChartPoint.ArcStartPointXPx property

Hämtar x-koordinaten för startpunkten för pajsektionen efter att ha anropat metoden Chart.Calculate(). Gäller för Pie- och Doughnut-diagram.

```csharp
public float ArcStartPointXPx { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcStartPointXPxDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

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

            // Visa värdet för ArcStartPointXPx
            Console.WriteLine("ArcStartPointXPx for first point: " + point.ArcStartPointXPx);

            // Obs: ArcStartPointXPx är skrivskyddad, så vi kan inte sätta den direkt
            // Istället kan vi demonstrera hur den förändras när vi ändrar andra egenskaper

            // Ändra explosionsvärdet som påverkar pajskivans position
            point.Explosion = 20;
            chart.Calculate(); // Recalculate to update properties

            // Visa det nya värdet för ArcStartPointXPx efter explosionsändring
            Console.WriteLine("ArcStartPointXPx after explosion: " + point.ArcStartPointXPx);

            // Spara arbetsboken
            workbook.Save("ChartPointPropertyArcStartPointXPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


