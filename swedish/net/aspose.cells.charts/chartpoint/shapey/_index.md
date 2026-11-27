---
title: "ChartPoint.ShapeY"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar y-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagrammets höjd efter anrop av Chart.Calculate-metoden"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/shapey/
---
## ChartPoint.ShapeY property

Hämtar y-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagrammets höjd efter att ha anropat metoden Chart.Calculate().

```csharp
public int ShapeY { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeYDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att få formens positioner
            chart.Calculate();

            // Hämta den första punkten i den första serien.
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa det aktuella ShapeY‑värdet (1/4000 av diagrammets höjd)
            Console.WriteLine("Current ShapeY value: " + point.ShapeY);

            // Obs: ShapeY är skrivskyddad, så vi kan inte sätta den direkt
            // För att ändra positionen måste vi modifiera de underliggande data eller diagrammets egenskaper

            // Demonstrera hur ShapeY relaterar till den faktiska positionen
            Console.WriteLine("ShapeY in pixels: " + point.ShapeYPx);
            Console.WriteLine("Chart height in pixels: " + (point.ShapeYPx * 4000 / point.ShapeY));

            // Spara resultatet
            workbook.Save("ChartPointPropertyShapeYDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


