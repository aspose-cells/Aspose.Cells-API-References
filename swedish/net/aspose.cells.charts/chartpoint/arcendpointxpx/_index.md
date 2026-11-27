---
title: "ChartPoint.ArcEndPointXPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar x-koordinaten för slutpunkten för pajsektionen efter att ha anropat metoden Chart.Calculate. Gäller för Pie- och Doughnut-diagram."
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/arcendpointxpx/
---
## ChartPoint.ArcEndPointXPx property

Hämtar x-koordinaten för slutpunkten för pajsektionen efter att ha anropat metoden Chart.Calculate(). Gäller för Pie- och Doughnut-diagram.

```csharp
public float ArcEndPointXPx { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcEndPointXPxDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att säkerställa att egenskaperna är fyllda
            chart.Calculate();

            // Hämta den första diagrampunkten
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa ArcEndPointXPx-värdet
            Console.WriteLine("ArcEndPointXPx: " + point.ArcEndPointXPx);

            // Obs: ArcEndPointXPx är skrivskyddad, så vi kan inte sätta den direkt
            // För att ändra slutpunkten måste vi ändra diagramdata eller egenskaper som påverkar pajskivan
            
            // Exempel på hur ändring av data påverkar ArcEndPointXPx
            worksheet.Cells["B2"].PutValue(60); // Increase Apple's value
            chart.Calculate(); // Recalculate chart

            // Visa det nya ArcEndPointXPx-värdet efter datändring
            Console.WriteLine("New ArcEndPointXPx after data change: " + point.ArcEndPointXPx);

            // Spara arbetsboken
            workbook.Save("ChartPointPropertyArcEndPointXPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


