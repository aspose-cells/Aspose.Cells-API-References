---
title: "ChartPoint.ShapeWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar bredden i enheter av 1/4000 av diagrammets bredd efter att ha anropat Chart.Calculate‑metoden"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/shapewidth/
---
## ChartPoint.ShapeWidth property

Hämtar bredden i enheter av 1/4000 av diagrammets bredd efter att ha anropat metoden Chart.Calculate().

```csharp
public int ShapeWidth { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeWidthDemo
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
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Beräkna diagrammet för att säkerställa att formegenskaperna är tillgängliga.
            chart.Calculate();
            
            // Hämta den första diagrampunkten i den första serien
            ChartPoint point = chart.NSeries[0].Points[0];
            
            // Visa det aktuella ShapeWidth‑värdet (i 1/4000 av diagrammets bredd)
            Console.WriteLine("Current ShapeWidth value: " + point.ShapeWidth);
            
            // Visa bredden i pixlar
            Console.WriteLine("Shape width in pixels: " + point.ShapeWidthPx);
            
            // Obs: ShapeWidth är skrivskyddad, så vi kan inte sätta den direkt
            // För att ändra bredden skulle vi behöva ändra diagrammets storlek eller andra egenskaper
            
            // Spara resultatet
            workbook.Save("ChartPointShapeWidthDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


