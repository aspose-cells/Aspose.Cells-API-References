---
title: "PatternFill.ForeTransparency"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PatternFill-Eigenschaft. Ruft die Transparenz der Vordergrundfarbe ab oder legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/patternfill/foretransparency/
---
## PatternFill.ForeTransparency property

Liest oder setzt die Transparenz der Vordergrundfarbe.

```csharp
public double ForeTransparency { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForeTransparencyDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Rechteckform hinzu, um die Musterfüllung zu demonstrieren
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // Setzen Sie den Fülltyp auf Muster
            shape.Fill.FillType = FillType.Pattern;

            // Holen Sie die PatternFill-Instanz
            PatternFill patternFill = shape.Fill.PatternFill;

            // Konfiguriere die PatternFill-Eigenschaften
            patternFill.Pattern = FillPattern.Solid;
            patternFill.ForegroundColor = Color.Red;
            patternFill.BackgroundColor = Color.Blue;

            try
            {
                // Zeige den anfänglichen ForeTransparency-Wert an
                Console.WriteLine("Initial ForeTransparency value: " + patternFill.ForeTransparency);

                // Setze einen neuen ForeTransparency-Wert (50 % Transparenz)
                patternFill.ForeTransparency = 0.5;

                // Zeige den aktualisierten ForeTransparency-Wert an
                Console.WriteLine("Updated ForeTransparency value: " + patternFill.ForeTransparency);

                // Speichere die Arbeitsmappe
                workbook.Save("ForeTransparencyDemo.xlsx");
                Console.WriteLine("ForeTransparency demonstration completed successfully.");
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

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


