---
title: "ChartPoint.ShapeYPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar y-koordinaten för det övre vänstra hörnet i pixelenheter efter anrop av Chart.Calculate-metoden."
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/shapeypx/
---
## ChartPoint.ShapeYPx property

Hämtar y-koordinaten för det övre vänstra hörnet i pixelenheter efter att ha anropat metoden Chart.Calculate().

```csharp
public int ShapeYPx { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeYPxDemo
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

            // Hämta första punkten i den första serien
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa aktuell Y-position i pixlar
            Console.WriteLine("Current ShapeYPx value: " + point.ShapeYPx);

            // Obs: ShapeYPx är skrivskyddad, så vi kan inte sätta den direkt
            // För att ändra positionen måste vi modifiera diagrammets storlek/position eller data

            // Demonstrera effekten genom att ändra diagrammets position, vilket kommer att påverka punktpositionerna
            chart.Move(2, 3, 17, 11); // Move chart to row 2, column 3
            chart.Calculate(); // Recalculate to update positions

            // Visa ny Y-position efter diagramförflyttning
            Console.WriteLine("New ShapeYPx value after chart movement: " + point.ShapeYPx);

            // Spara resultatet
            workbook.Save("ChartPointShapeYPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


