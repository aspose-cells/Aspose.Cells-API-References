---
title: "Line.Transparency"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Line property. Gibt den Transparenzgrad der Linie zurück oder legt ihn fest, als Wert von 0,0 undurchsichtig bis 1,0 klar"
type: docs
url: /de/net/aspose.cells.drawing/line/transparency/
---
## Line.Transparency property

Gibt den Transparenzgrad der Linie zurück oder legt ihn fest, als Wert von 0.0 (undurchsichtig) bis 1.0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyTransparencyDemo
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
                // Fügen Sie ein Liniendiagramm hinzu, um Linieneigenschaften zu demonstrieren
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B3", true);

                // Rufen Sie die Linieneigenschaften aus dem Diagramm‑Serienrand ab
                Line line = chart.NSeries[0].Border;

                // Zeige den aktuellen Transparenzwert an
                Console.WriteLine("Current Transparency: " + line.Transparency);

                // Setzen Sie einen neuen Transparency-Wert (0,0 = undurchsichtig, 1,0 = klar)
                line.Transparency = 0.5;
                Console.WriteLine("Updated Transparency: " + line.Transparency);

                // Speichere die Arbeitsmappe
                workbook.Save("TransparencyDemo.xlsx");
                Console.WriteLine("Transparency property demonstrated successfully.");
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


