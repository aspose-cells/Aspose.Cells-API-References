---
title: "MsoLineFormatHelper.IsVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoLineFormatHelper-Eigenschaft. Gibt an, ob das Objekt sichtbar ist"
type: docs
url: /de/net/aspose.cells.drawing/msolineformathelper/isvisible/
---
## MsoLineFormatHelper.IsVisible property

Gibt an, ob das Objekt sichtbar ist.

```csharp
public bool IsVisible { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyIsVisibleDemo
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

                // Zeige den aktuellen IsVisible-Wert an
                Console.WriteLine("Current IsVisible: " + lineFormat.IsVisible);

                // Setze einen neuen IsVisible-Wert (da er les-/schreibbar ist)
                lineFormat.IsVisible = false;
                Console.WriteLine("Updated IsVisible: " + lineFormat.IsVisible);

                // Zeigen, wie die Eigenschaft das Verhalten beeinflusst
                Console.WriteLine("Line visibility has been updated to: " + lineFormat.IsVisible);

                // Ergebnis speichern
                workbook.Save("IsVisibleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line visibility.");
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


