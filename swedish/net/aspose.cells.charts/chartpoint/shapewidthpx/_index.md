---
title: "ChartPoint.ShapeWidthPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint egenskap. Hämtar bredden i pixelenheter efter att ha anropat Chart.Calculate‑metoden"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/shapewidthpx/
---
## ChartPoint.ShapeWidthPx property

Hämtar bredden i enheter av pixlar efter att ha anropat metoden Chart.Calculate().

```csharp
public int ShapeWidthPx { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeWidthPxDemo
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

            // Beräkna diagrammet för att säkerställa att formegenskaperna är tillgängliga.
            chart.Calculate();

            // Hämta den första diagrampunkten från den första serien
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa den aktuella bredden på diagrampunktsformen i pixlar
            Console.WriteLine("Current ShapeWidthPx value: " + point.ShapeWidthPx);

            // Obs: ShapeWidthPx är skrivskyddad, så vi kan inte sätta den direkt
            // För att ändra bredden måste vi modifiera diagrammets storlek eller andra egenskaper
            // detta skulle påverka punktens bredd under nästa Calculate()

            // Ändra diagrammets bredd för att demonstrera hur det påverkar ShapeWidthPx
            chart.ChartObject.Width = 1000;
            chart.Calculate();

            // Visa den nya bredden efter diagramändring
            Console.WriteLine("New ShapeWidthPx value after chart resize: " + point.ShapeWidthPx);

            // Spara resultatet
            workbook.Save("ChartPointPropertyShapeWidthPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


