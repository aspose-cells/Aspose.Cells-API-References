---
title: "MsoLineFormatHelper.Transparency"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoLineFormatHelper-Eigenschaft. Gibt den Transparenzgrad der angegebenen Füllung zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (klar)"
type: docs
url: /de/net/aspose.cells.drawing/msolineformathelper/transparency/
---
## MsoLineFormatHelper.Transparency property

Gibt den Transparenzgrad der angegebenen Füllung zurück oder setzt ihn, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Erstelle ein Beispiel-Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten hinzu, um das Beispiel sinnvoll zu machen.
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Erstelle eine Form, um die Linienformatierung zu demonstrieren
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // Hole das Linienformat
                MsoLineFormat lineFormat = shape.LineFormat;

                // Zeige den aktuellen Transparenzwert an
                Console.WriteLine("Current Transparency: " + lineFormat.Transparency);

                // Setze einen neuen Transparenzwert (da er les- und schreibbar ist)
                lineFormat.Transparency = 0.5;
                Console.WriteLine("Updated Transparency: " + lineFormat.Transparency);

                // Zeigen, wie die Eigenschaft das Verhalten beeinflusst
                Console.WriteLine("Line transparency has been updated to: " + lineFormat.Transparency);

                // Ergebnis speichern
                workbook.Save("TransparencyDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line transparency.");
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

* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


