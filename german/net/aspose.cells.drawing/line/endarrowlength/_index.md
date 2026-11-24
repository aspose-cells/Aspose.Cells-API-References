---
title: "Line.EndArrowLength"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Line‑Eigenschaft. Gibt die Länge der Pfeilspitze am Ende einer Linie an"
type: docs
url: /de/net/aspose.cells.drawing/line/endarrowlength/
---
## Line.EndArrowLength property

Gibt die Länge der Pfeilspitze für das Ende einer Linie an.

```csharp
public MsoArrowheadLength EndArrowLength { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Erstelle ein Beispiel-Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten hinzu, um das Beispiel sinnvoll zu machen.
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Values");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            try
            {
                // Fügen Sie ein Diagramm hinzu, um Linieneigenschaften zu demonstrieren
                int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
                Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B3", true);

                // Rufen Sie die Linieneigenschaften aus dem Diagramm‑Serienrand ab
                Line line = chart.NSeries[0].Border;

                // Setzen Sie einen Pfeilspitzentyp, um EndArrowLength zu demonstrieren
                line.EndType = MsoArrowheadStyle.Arrow;

                // Zeigen Sie den aktuellen EndArrowLength-Wert an
                Console.WriteLine("Current EndArrowLength: " + line.EndArrowLength);

                // Setzen Sie einen neuen EndArrowLength-Wert
                line.EndArrowLength = MsoArrowheadLength.Long;
                Console.WriteLine("Updated EndArrowLength: " + line.EndArrowLength);

                // Speichere die Arbeitsmappe
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

### Siehe auch

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


