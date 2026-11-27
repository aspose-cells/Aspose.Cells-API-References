---
title: "ChartPoint.InnerRadiusPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar den inre radien för donutsegmentet i pixelenheter efter anrop av metoden Chart.Calculate. Gäller för donutdiagram."
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/innerradiuspx/
---
## ChartPoint.InnerRadiusPx property

Hämtar den inre radien för donutsegmentet i pixelenheter efter anrop av metoden Chart.Calculate(). Gäller för donutdiagram.

```csharp
[Obsolete("Use ChartPoint.DoughnutInnerRadius property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerRadiusPx { get; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen ChartPoint.DoughnutInnerRadius. Denna egenskap kommer att tas bort 12 månader efter juni 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerRadiusPxDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att få egenskaperna för diagrampunkterna.
            chart.Calculate();

            // Hämta den första diagrampunkten från den första serien
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa det aktuella inre radievärdet (skrivskyddad egenskap).
            Console.WriteLine("Current InnerRadiusPx value: " + point.InnerRadiusPx);

            // Obs: InnerRadiusPx är skrivskyddad, så vi kan inte sätta den direkt.
            // För att ändra den inre radien måste vi justera storleken på donutens hål.
            chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size

            // Beräkna om diagrammet för att uppdatera egenskaperna
            chart.Calculate();

            // Visa det nya inre radievärdet efter att donutens hålstorlek har ändrats.
            Console.WriteLine("New InnerRadiusPx value after changing DoughnutHoleSize: " + point.InnerRadiusPx);

            // Spara resultatet
            workbook.Save("ChartPointPropertyInnerRadiusPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


