---
title: "Line.BeginArrowLength"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Linieneigenschaft. Gibt die Länge der Pfeilspitze für den Anfang einer Linie an"
type: docs
url: /de/net/aspose.cells.drawing/line/beginarrowlength/
---
## Line.BeginArrowLength property

Gibt die Länge der Pfeilspitze für den Anfang einer Linie an.

```csharp
public MsoArrowheadLength BeginArrowLength { get; set; }
```

### Beispiele

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
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einfach Daten für ein Diagramm vorbereiten
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

                // Setze die BeginArrowLength auf Long
                seriesLine.BeginArrowLength = MsoArrowheadLength.Long;

                // Lese und zeige den aktuellen BeginArrowLength-Wert an
                Console.WriteLine("BeginArrowLength value: " + seriesLine.BeginArrowLength);

                // Speichere die Arbeitsmappe (optional, nur um die Demo zu vervollständigen)
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

### Siehe auch

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


