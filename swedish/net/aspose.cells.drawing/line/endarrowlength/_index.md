---
title: "Line.EndArrowLength"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Line-egenskap. Anger längden på pilspetsen för slutet av en linje"
type: docs
url: /sv/net/aspose.cells.drawing/line/endarrowlength/
---
## Line.EndArrowLength property

Anger längden på pilspetsen för slutet av en linje.

```csharp
public MsoArrowheadLength EndArrowLength { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyEndArrowLengthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa ett exempelark
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data för att göra exemplet meningsfullt
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Values");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            try
            {
                // Lägg till ett diagram för att demonstrera linjeegenskaper
                int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
                Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B3", true);

                // Hämta linjeegenskaperna från diagramseriens kant
                Line line = chart.NSeries[0].Border;

                // Ställ in en pilspets-typ för att demonstrera EndArrowLength
                line.EndType = MsoArrowheadStyle.Arrow;

                // Visa det aktuella värdet för EndArrowLength
                Console.WriteLine("Current EndArrowLength: " + line.EndArrowLength);

                // Ställ in ett nytt EndArrowLength‑värde
                line.EndArrowLength = MsoArrowheadLength.Long;
                Console.WriteLine("Updated EndArrowLength: " + line.EndArrowLength);

                // Spara arbetsboken
                workbook.Save("EndArrowLengthDemo.xlsx");
                Console.WriteLine("EndArrowLength property demonstrated successfully.");
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


