---
title: "ChartPoint.ShapeHeightPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint‑egenskap. Hämtar höjden i pixelenheter efter anrop av Chart.Calculate‑metoden"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/shapeheightpx/
---
## ChartPoint.ShapeHeightPx property

Hämtar höjden i enheter av pixlar efter att anropa metoden Chart.Calculate().

```csharp
public int ShapeHeightPx { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeHeightPxDemo
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

            // Beräkna diagrammet för att få formens dimensioner
            chart.Calculate();

            // Hämta den första diagrampunkten från den första serien
            ChartPoint chartPoint = chart.NSeries[0].Points[0];

            // Visa den aktuella höjden på diagrampunktsformen i pixlar
            Console.WriteLine("Current ShapeHeightPx value: " + chartPoint.ShapeHeightPx);

            // Obs: ShapeHeightPx är skrivskyddad, så vi kan inte sätta den direkt
            // För att ändra höjden måste vi modifiera diagramstorleken eller datavärdena
            // och beräkna om diagrammet

            // Ändra datavärdet som kommer att påverka diagrampunktsstorleken
            worksheet.Cells["B2"].PutValue(50);
            chart.Calculate();

            // Visa den nya höjden efter att datan har ändrats
            Console.WriteLine("New ShapeHeightPx value after data change: " + chartPoint.ShapeHeightPx);

            // Spara arbetsboken
            workbook.Save("ChartPointShapeHeightPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


