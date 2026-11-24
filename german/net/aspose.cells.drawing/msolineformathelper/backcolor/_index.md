---
title: "MsoLineFormatHelper.BackColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoLineFormatHelper-Eigenschaft. Gibt die Hintergrundfarbe der Randlinie zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/msolineformathelper/backcolor/
---
## MsoLineFormatHelper.BackColor property

Liest und setzt die Hintergrundfarbe der Randlinie.

```csharp
public Color BackColor { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyBackColorDemo
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

                // Zeige den aktuellen BackColor-Wert an
                Console.WriteLine("Current BackColor: " + lineFormat.BackColor);

                // Setze einen neuen BackColor-Wert (da er les-/schreibbar ist)
                lineFormat.BackColor = Color.LightBlue;
                Console.WriteLine("Updated BackColor: " + lineFormat.BackColor);

                // Zeigen, wie die Eigenschaft das Verhalten beeinflusst
                Console.WriteLine("Line back color has been updated to: " + lineFormat.BackColor);

                // Ergebnis speichern
                workbook.Save("BackColorDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line back color.");
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


