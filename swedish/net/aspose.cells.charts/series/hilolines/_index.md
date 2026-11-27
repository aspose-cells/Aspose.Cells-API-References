---
title: "Series.HiLoLines"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series‑egenskap. Returnerar ett HiLoLines‑objekt som representerar hög‑låg‑linjerna för en serie i ett linjediagram. Gäller endast linjediagram."
type: docs
url: /sv/net/aspose.cells.charts/series/hilolines/
---
## Series.HiLoLines property

Returnerar ett HiLoLines-objekt som representerar hög-låg-linjerna för en serie i ett linjediagram. Gäller endast linjediagram.

```csharp
public Line HiLoLines { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class SeriesPropertyHiLoLinesDemo
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

            worksheet.Cells["B1"].PutValue("High");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(150);
            worksheet.Cells["B5"].PutValue(110);

            worksheet.Cells["C1"].PutValue("Low");
            worksheet.Cells["C2"].PutValue(80);
            worksheet.Cells["C3"].PutValue(60);
            worksheet.Cells["C4"].PutValue(100);
            worksheet.Cells["C5"].PutValue(70);

            // Lägg till ett linjediagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B1:B5", true);
            chart.NSeries.Add("C1:C5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Aktivera HiLoLines för den första serien
            Series series = chart.NSeries[0];
            series.HasHiLoLines = true;

            // Kom åt och ändra HiLoLines‑egenskaper
            Line hiLoLines = series.HiLoLines;
            Console.WriteLine("HiLoLines visibility: " + hiLoLines.IsVisible);

            // Anpassa HiLoLines‑utseende
            hiLoLines.Color = System.Drawing.Color.Red;
            hiLoLines.Weight = WeightType.MediumLine;
            hiLoLines.DashType = MsoLineDashStyle.DashDot;
            hiLoLines.IsVisible = true;

            // Spara resultatet
            workbook.Save("SeriesPropertyHiLoLinesDemo.xlsx");
        }
    }
}
```

### Se även

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


