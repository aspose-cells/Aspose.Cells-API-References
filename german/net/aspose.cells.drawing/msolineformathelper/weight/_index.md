---
title: "MsoLineFormatHelper.Weight"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoLineFormatHelper-Eigenschaft. Gibt das Gewicht der Linie in pt zurück oder legt es fest"
type: docs
url: /de/net/aspose.cells.drawing/msolineformathelper/weight/
---
## MsoLineFormatHelper.Weight property

Gibt das Gewicht der Linie zurück oder setzt es, in pt-Einheiten.

```csharp
public double Weight { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyWeightDemo
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

                // Zeige den aktuellen Weight-Wert an
                Console.WriteLine("Current Line Weight: " + lineFormat.Weight);

                // Setze einen neuen Weight-Wert (da er les-/schreibbar ist)
                lineFormat.Weight = 2.5;
                Console.WriteLine("Updated Line Weight: " + lineFormat.Weight);

                // Zeigen, wie die Eigenschaft das Verhalten beeinflusst
                Console.WriteLine("Line weight has been updated to: " + lineFormat.Weight);

                // Ergebnis speichern
                workbook.Save("WeightDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line weight.");
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


