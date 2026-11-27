---
title: "ChartPoint.ShapeXPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint egenskap. Hämtar x‑koordinaten för det övre vänstra hörnet i pixelenheter efter att ha anropat metoden Chart.Calculate."
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/shapexpx/
---
## ChartPoint.ShapeXPx property

Hämtar x-koordinaten för det övre vänstra hörnet i pixelenheter efter att ha anropat metoden Chart.Calculate().

```csharp
public int ShapeXPx { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeXPxDemo
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

            // Beräkna diagrammet för att få formpositioner.
            chart.Calculate();

            // Hämta den första diagrampunkten från den första serien
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa den aktuella X‑positionen i pixlar.
            Console.WriteLine("Current ShapeXPx value: " + point.ShapeXPx);

            // Obs: ShapeXPx är skrivskyddad, så vi kan inte sätta den direkt.
            // För att ändra positionen måste vi ändra diagrammets storlek/position eller data.

            // Visa hur egenskapen förändras när vi ändrar diagrammet.
            Console.WriteLine("\nChanging chart position...");
            chart.ChartObject.Left = 3;
            chart.ChartObject.Top = 2;
            chart.Calculate(); // Recalculate to update positions

            Console.WriteLine("New ShapeXPx value after chart move: " + point.ShapeXPx);

            // Spara resultatet
            workbook.Save("ChartPointPropertyShapeXPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


