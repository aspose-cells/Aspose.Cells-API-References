---
title: "Line.IsAutomaticColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Line property. Gibt an, ob die Farbe der Linie automatisch zugewiesen wird"
type: docs
url: /de/net/aspose.cells.drawing/line/isautomaticcolor/
---
## Line.IsAutomaticColor property

Gibt an, ob die Farbe der Linie automatisch zugewiesen wird.

```csharp
public bool IsAutomaticColor { get; }
```

### Beispiele

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
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für ein Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Ein Liniendiagramm hinzufügen
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";

                // Greifen Sie auf die Linie (Rand) der ersten Serie zu
                Line seriesLine = chart.NSeries[0].Border;

                // Lesen und zeigen Sie den Wert der IsAutomaticColor-Eigenschaft an
                Console.WriteLine("IsAutomaticColor value: " + seriesLine.IsAutomaticColor);

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


