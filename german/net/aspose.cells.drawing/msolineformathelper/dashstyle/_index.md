---
title: "MsoLineFormatHelper.DashStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoLineFormatHelper-Eigenschaft. Gibt den Strichstil für die angegebene Linie zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/msolineformathelper/dashstyle/
---
## MsoLineFormatHelper.DashStyle property

Liest oder setzt den Strichstil für die angegebene Linie.

```csharp
public MsoLineDashStyle DashStyle { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyDashStyleDemo
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

                // Zeige den aktuellen DashStyle-Wert an
                Console.WriteLine("Current DashStyle: " + lineFormat.DashStyle);

                // Setze einen neuen DashStyle-Wert (da er les-/schreibbar ist)
                lineFormat.DashStyle = MsoLineDashStyle.DashDot;
                Console.WriteLine("Updated DashStyle: " + lineFormat.DashStyle);

                // Zeigen, wie die Eigenschaft das Verhalten beeinflusst
                Console.WriteLine("Line dash style has been updated to: " + lineFormat.DashStyle);

                // Ergebnis speichern
                workbook.Save("DashStyleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line dash style.");
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

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


