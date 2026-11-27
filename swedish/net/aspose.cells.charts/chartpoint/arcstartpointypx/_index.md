---
title: "ChartPoint.ArcStartPointYPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar y-koordinaten för startpunkten för pajavsnittet efter anrop av metoden Chart.Calculate. Gäller för paj- och munkdiagram."
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/arcstartpointypx/
---
## ChartPoint.ArcStartPointYPx property

Hämtar y-koordinaten för startpunkten för pajsektionen efter att anropa metoden Chart.Calculate(). Gäller för Pie- och Doughnut-diagram.

```csharp
public float ArcStartPointYPx { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcStartPointYPxDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att få formens positioner.
            chart.Calculate();

            // Hämta den första diagrampunkten
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa det aktuella värdet för ArcStartPointYPx
            Console.WriteLine("Current ArcStartPointYPx value: " + point.ArcStartPointYPx);

            // Obs: ArcStartPointYPx är skrivskyddad, så vi kan inte sätta den direkt
            // Istället kommer vi att demonstrera hur ändring av andra egenskaper påverkar ArcStartPointYPx

            // Ändra explosionsvärdet för att modifiera positionen för pajskivan
            point.Explosion = 20;

            // Beräkna om diagrammet för att uppdatera positionerna
            chart.Calculate();

            // Visa det nya ArcStartPointYPx‑värdet efter att explosionsvärdet har ändrats
            Console.WriteLine("New ArcStartPointYPx after explosion change: " + point.ArcStartPointYPx);

            // Spara arbetsboken
            workbook.Save("ChartPointPropertyArcStartPointYPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


