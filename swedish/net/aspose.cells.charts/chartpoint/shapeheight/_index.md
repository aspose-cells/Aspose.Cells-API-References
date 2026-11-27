---
title: "ChartPoint.ShapeHeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar höjden i enheter av 1/4000 av diagrammets höjd efter anrop av metoden Chart.Calculate."
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/shapeheight/
---
## ChartPoint.ShapeHeight property

Hämtar höjden i enheter av 1/4000 av diagrammets höjd efter att anropa metoden Chart.Calculate().

```csharp
public int ShapeHeight { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeHeightDemo
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

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att säkerställa att formegenskaperna är tillgängliga.
            chart.Calculate();

            // Hämta den första punkten i den första serien.
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa det aktuella ShapeHeight‑värdet (i 1/4000 av diagrammets höjd).
            Console.WriteLine("Current ShapeHeight value: " + point.ShapeHeight);

            // Obs: ShapeHeight är skrivskyddad, så vi kan inte sätta den direkt.
            // För att ändra höjden måste vi modifiera diagrammets storlek eller andra egenskaper.

            // Demonstrera effekten genom att ändra diagrammets höjd.
            Console.WriteLine("Original chart height: " + chart.ChartObject.Height);
            chart.ChartObject.Height = 400;
            chart.Calculate(); // Recalculate to update shape properties

            // Visa det nya ShapeHeight‑värdet efter att diagrammets höjd har ändrats.
            Console.WriteLine("New ShapeHeight value after chart resize: " + point.ShapeHeight);

            // Spara resultatet
            workbook.Save("ChartPointPropertyShapeHeightDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


