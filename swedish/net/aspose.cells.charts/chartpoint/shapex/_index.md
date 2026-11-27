---
title: "ChartPoint.ShapeX"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint‑egenskap. Hämtar x‑koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagrammets bredd efter anrop av Chart.Calculate‑metoden"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/shapex/
---
## ChartPoint.ShapeX property

Hämtar x-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagrammets bredd efter att ha anropat metoden Chart.Calculate().

```csharp
public int ShapeX { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeXDemo
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

            // Beräkna diagrammet för att säkerställa att ShapeX fylls i
            chart.Calculate();

            // Hämta den första punkten i den första serien.
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa ShapeX‑värdet (1/4000 av diagrammets bredd)
            Console.WriteLine("ShapeX value (1/4000 units): " + point.ShapeX);
            Console.WriteLine("ShapeX value (pixels): " + point.ShapeXPx);

            // Demonstrera hur man använder ShapeX för att placera element relativt till diagrampunkten
            // Obs: Eftersom ShapeX är skrivskyddad kan vi inte ändra den direkt,
            // men vi kan också använda den för att placera andra element
            if (point.ShapeX > 0)
            {
                // Lägg till en textruta som är justerad med diagrampunktens X‑position
                Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(
                    point.ShapeXPx, 100, 100, 50, 100, 50);
                textBox.Text = "Point 1";
            }

            // Spara resultatet
            workbook.Save("ChartPointShapeXDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


