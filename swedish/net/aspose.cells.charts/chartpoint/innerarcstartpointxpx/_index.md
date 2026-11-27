---
title: "ChartPoint.InnerArcStartPointXPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar x-koordinaten för startpunkten för pajsektionen efter att ha anropat metoden Chart.Calculate. Gäller för Doughnut-diagram"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/innerarcstartpointxpx/
---
## ChartPoint.InnerArcStartPointXPx property

Hämtar x-koordinaten för startpunkten för pajsektionen efter att ha anropat metoden Chart.Calculate(). Gäller för Doughnut-diagrammet.

```csharp
public float InnerArcStartPointXPx { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcStartPointXPxDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett doughnut-diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att få formegenskaperna
            chart.Calculate();

            // Hämta den första diagrampunkten
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa värdet InnerArcStartPointXPx
            Console.WriteLine("InnerArcStartPointXPx: " + point.InnerArcStartPointXPx);

            // Obs: InnerArcStartPointXPx är skrivskyddad, så vi kan inte sätta den direkt
            // För att ändra positionen måste vi ändra diagrammets storlek eller storleken på doughnut-hålet

            // Spara arbetsboken
            workbook.Save("ChartPointPropertyInnerArcStartPointXPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


