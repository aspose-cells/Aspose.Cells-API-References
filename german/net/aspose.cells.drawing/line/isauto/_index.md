---
title: "Line.IsAuto"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Line property. Gibt an, ob dieser Linienstil automatisch zugewiesen wird"
type: docs
url: /de/net/aspose.cells.drawing/line/isauto/
---
## Line.IsAuto property

Gibt an, ob dieser Linienstil automatisch zugewiesen wird.

```csharp
public bool IsAuto { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyIsAutoDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Ein Liniendiagramm hinzufügen
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
                Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

                // Diagrammdatenbereich festlegen
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";

                // Greifen Sie auf die Linieneigenschaften der Serie zu
                Aspose.Cells.Charts.Series series = chart.NSeries[0];
                Line line = series.Border;

                // Zeigen Sie den aktuellen IsAuto-Wert an
                Console.WriteLine("Initial IsAuto value: " + line.IsAuto);

                // Setzen Sie IsAuto auf true
                line.IsAuto = true;
                Console.WriteLine("After setting to true, IsAuto value: " + line.IsAuto);

                // Setzen Sie IsAuto auf false
                line.IsAuto = false;
                Console.WriteLine("After setting to false, IsAuto value: " + line.IsAuto);

                // Speichere die Arbeitsmappe
                workbook.Save("IsAutoDemo.xlsx");
                Console.WriteLine("IsAuto property has been demonstrated successfully.");
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


