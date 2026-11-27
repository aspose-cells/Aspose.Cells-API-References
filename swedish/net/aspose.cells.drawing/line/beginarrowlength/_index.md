---
title: "Line.BeginArrowLength"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Linjeegenskap. Anger längden på pilspetsen för början av en linje"
type: docs
url: /sv/net/aspose.cells.drawing/line/beginarrowlength/
---
## Line.BeginArrowLength property

Anger längden på pilspetsen för början av en linje.

```csharp
public MsoArrowheadLength BeginArrowLength { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class LinePropertyBeginArrowLengthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Förbered enkel data för ett diagram
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Lägg till ett linjediagram
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";

                // Kom åt linjen (ramen) för den första serien
                Line seriesLine = chart.NSeries[0].Border;

                // Ställ in BeginArrowLength till Long
                seriesLine.BeginArrowLength = MsoArrowheadLength.Long;

                // Läs och visa det aktuella BeginArrowLength-värdet
                Console.WriteLine("BeginArrowLength value: " + seriesLine.BeginArrowLength);

                // Spara arbetsboken (valfritt, bara för att slutföra demonstrationen)
                workbook.Save("BeginArrowLengthDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


