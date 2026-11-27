---
title: "ChartPoint.BorderWidthPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar kantens bredd i pixelenheter efter anrop av Chart.Calculate-metoden."
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/borderwidthpx/
---
## ChartPoint.BorderWidthPx property

Hämtar bredden på kanten i enheter av pixlar efter att ha anropat metoden Chart.Calculate().

```csharp
public int BorderWidthPx { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ChartPointPropertyBorderWidthPxDemo
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
            worksheet.Cells["A5"].PutValue("Q4");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2100);

            // Lägg till ett diagram och ange dess dataintervall
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Beräkna diagrammet för att säkerställa att egenskaperna är fyllda
            chart.Calculate();

            // Hämta den första diagrampunkten i den första serien
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa den aktuella kantbredden
            Console.WriteLine("Current BorderWidthPx value: " + point.BorderWidthPx);

            // Obs: BorderWidthPx är skrivskyddad, så vi kan inte sätta den direkt
            // Istället kan vi ändra kanten via egenskapen Border
            if (point.Border != null)
            {
                // Ändra kantbredden genom att sätta vikten med enumen WeightType
                point.Border.Weight = WeightType.MediumLine; // Medium weight border
            }

            // Beräkna om för att uppdatera värdet BorderWidthPx
            chart.Calculate();

            // Visa den nya kantbredden i pixlar
            Console.WriteLine("New BorderWidthPx value after modification: " + point.BorderWidthPx);

            // Spara arbetsboken
            workbook.Save("ChartPointPropertyBorderWidthPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


