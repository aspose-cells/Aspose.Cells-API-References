---
title: "ChartPoint.RadiusPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar radien för bubbeldiagram eller donut i pixelenheter efter anrop av metoden Chart.Calculate"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/radiuspx/
---
## ChartPoint.RadiusPx property

Hämtar radien för bubbla, paj eller doughnut i enheter av pixlar efter att anropa metoden Chart.Calculate().

```csharp
public int RadiusPx { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyRadiusPxDemo
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

            // Visa det aktuella radievärdet
            Console.WriteLine("Current RadiusPx value: " + point.RadiusPx);

            // Obs: RadiusPx är skrivskyddad, så vi kan inte sätta den direkt
            // För att ändra radien måste vi justera diagrammets storlek eller andra egenskaper
            // som påverkar punktens storlek indirekt

            // Exempel på hur ändring av diagramstorlek påverkar radien
            Console.WriteLine("\nChanging chart size to demonstrate radius change...");
            chart.ChartObject.Width = 800;
            chart.ChartObject.Height = 600;
            chart.Calculate();

            // Visa det nya radievärdet efter diagramändring
            Console.WriteLine("New RadiusPx value after chart resize: " + point.RadiusPx);

            // Spara resultatet
            workbook.Save("ChartPointPropertyRadiusPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


