---
title: "MsoLineFormatHelper.Style"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoLineFormatHelper-Eigenschaft. Gibt ein Style-Objekt zurück, das den Stil des angegebenen Bereichs darstellt"
type: docs
url: /de/net/aspose.cells.drawing/msolineformathelper/style/
---
## MsoLineFormatHelper.Style property

Gibt ein Style-Objekt zurück, das den Stil des angegebenen Bereichs darstellt.

```csharp
public MsoLineStyle Style { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyStyleDemo
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

                // Hole das Linienformat direkt (MsoLineFormatHelper scheint eine Hilfsklasse zu sein)
                // Da wir MsoLineFormatHelper nicht direkt instanziieren können, arbeiten wir mit der LineFormat-Eigenschaft
                MsoLineFormat lineFormat = shape.LineFormat;

                // Zeige den aktuellen Style-Wert an
                Console.WriteLine("Current Line Style: " + lineFormat.Style);

                // Setze einen neuen Stil (da Style les-/schreibbar ist)
                lineFormat.Style = MsoLineStyle.ThickBetweenThin;
                Console.WriteLine("Updated Line Style: " + lineFormat.Style);

                // Zeigen, wie die Eigenschaft das Verhalten beeinflusst
                Console.WriteLine("Line style has been updated to: " + lineFormat.Style);

                // Ergebnis speichern
                workbook.Save("LineStyleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line style.");
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

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


