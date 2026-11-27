---
title: "ChartPoint.ArcEndPointYPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar y‑koordinaten för slutpunkten för pajsektionen efter anrop av metoden Chart.Calculate. Gäller för paj- och donutdiagram."
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/arcendpointypx/
---
## ChartPoint.ArcEndPointYPx property

Hämtar y-koordinaten för slutpunkten för pajsektionen efter att anropa metoden Chart.Calculate(). Gäller för Pie- och Doughnut-diagram.

```csharp
public float ArcEndPointYPx { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcEndPointYPxDemo
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
            worksheet.Cells["B2"].PutValue(8000);
            worksheet.Cells["B3"].PutValue(12000);
            worksheet.Cells["B4"].PutValue(14000);

            // Lägg till ett pajdiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att få formens positioner.
            chart.Calculate();

            // Hämta den första diagrampunkten
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa det aktuella ArcEndPointYPx‑värdet.
            Console.WriteLine("Current ArcEndPointYPx value: " + point.ArcEndPointYPx);

            // Eftersom ArcEndPointYPx är skrivskyddad kan vi bara läsa den.
            // Följande rad skulle orsaka ett kompileringsfel:
            // point.ArcEndPointYPx = 150.5f;

            // Demonstrera hur denna egenskap påverkar pajdiagrammet.
            Console.WriteLine("Pie slice end point Y coordinate: " + point.ArcEndPointYPx + " pixels");

            // Spara arbetsboken
            workbook.Save("ChartPointPropertyArcEndPointYPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


