---
title: "ChartPoint.DoughnutInnerRadius"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar den inre radien av donut-skivan i pixelenheter efter att ha anropat Chart.Calculate‑metoden. Gäller för Doughnut-diagram"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/doughnutinnerradius/
---
## ChartPoint.DoughnutInnerRadius property

Hämtar den inre radien på doughnut‑segmentet i enheter av pixlar efter att ha anropat metoden Chart.Calculate(). Gäller för Doughnut-diagram.

```csharp
public int DoughnutInnerRadius { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyDoughnutInnerRadiusDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("C1");
            worksheet.Cells["A3"].PutValue("C2");
            worksheet.Cells["A4"].PutValue("C3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(5);

            // Lägg till ett doughnut-diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att få diagrampunkterna
            chart.Calculate();

            // Hämta den första diagrampunkten från den första serien
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa det aktuella DoughnutInnerRadius‑värdet
            Console.WriteLine("Current DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // Obs: DoughnutInnerRadius är skrivskyddad, så vi kan inte sätta den direkt
            // För att ändra den inre radien måste vi justera HoleSize‑egenskapen för diagrammet
            chart.FirstSliceAngle = 30; // Adjust the first slice angle instead since HoleSize isn't available

            // Beräkna om diagrammet för att uppdatera DoughnutInnerRadius
            chart.Calculate();

            // Visa det uppdaterade DoughnutInnerRadius‑värdet
            Console.WriteLine("Updated DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // Spara arbetsboken
            workbook.Save("DoughnutInnerRadiusDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


