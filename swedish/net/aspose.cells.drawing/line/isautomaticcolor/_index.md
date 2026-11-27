---
title: "Line.IsAutomaticColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Linjeegenskap. Anger om färgen på linjen är automatiskt tilldelad"
type: docs
url: /sv/net/aspose.cells.drawing/line/isautomaticcolor/
---
## Line.IsAutomaticColor property

Indikerar om linjens färg tilldelas automatiskt.

```csharp
public bool IsAutomaticColor { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LinePropertyIsAutomaticColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för ett diagram
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

                // Läs och visa värdet för IsAutomaticColor‑egenskapen
                Console.WriteLine("IsAutomaticColor value: " + seriesLine.IsAutomaticColor);

                // Spara arbetsboken
                workbook.Save("IsAutomaticColorDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


