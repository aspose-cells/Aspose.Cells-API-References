---
title: "Series.DropLines"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Returnerar ett Line-objekt som representerar droplinjer för en serie i ett linjediagram eller ett områdesdiagram. Gäller endast för linjediagram eller områdesdiagram"
type: docs
url: /sv/net/aspose.cells.charts/series/droplines/
---
## Series.DropLines property

Returnerar ett [`Line`](../../../aspose.cells.drawing/line/) objekt som representerar droplinjer för en serie i ett linjediagram eller ett områdesdiagram. Gäller endast för linjediagram eller områdesdiagram.

```csharp
public Line DropLines { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class SeriesPropertyDropLinesDemo
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

            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(180);
            worksheet.Cells["B5"].PutValue(210);

            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(90);
            worksheet.Cells["C3"].PutValue(130);
            worksheet.Cells["C4"].PutValue(160);
            worksheet.Cells["C5"].PutValue(190);

            // Lägg till ett linjediagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.Add("C2:C5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Aktivera droplinjer för diagrammet
            chart.NSeries[0].HasDropLines = true;
            chart.NSeries[1].HasDropLines = true;

            // Åtkomst till droplinjerna för den första serien
            Line dropLines = chart.NSeries[0].DropLines;

            // Visa aktuella droplinjeegenskaper
            Console.WriteLine("Drop line color: " + dropLines.Color);
            Console.WriteLine("Drop line style: " + dropLines.Style);
            Console.WriteLine("Drop line weight: " + dropLines.Weight);

            // Ändra droplinjeegenskaper
            dropLines.Color = System.Drawing.Color.Red;
            dropLines.Style = LineType.Solid;
            dropLines.Weight = WeightType.MediumLine;
            dropLines.DashType = MsoLineDashStyle.Solid;
            dropLines.IsVisible = true;

            // Spara arbetsboken
            workbook.Save("SeriesPropertyDropLinesDemo.xlsx");
        }
    }
}
```

### Se även

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


