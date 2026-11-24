---
title: "TextOptions.Spacing"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextOptions property. Gibt den Abstand zwischen Zeichen innerhalb eines Textabschnitts an"
type: docs
url: /de/net/aspose.cells.drawing.texts/textoptions/spacing/
---
## TextOptions.Spacing property

Gibt den Abstand zwischen Zeichen innerhalb eines Textlaufs an.

```csharp
public double Spacing { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertySpacingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 0, 100, 200);
            textBox.Text = "Sample Text with Spacing";

            // Rufe die Textoptionen des Textfelds ab
            TextOptions textOptions = textBox.TextOptions;

            // Zeige den aktuellen Abstandswert an
            Console.WriteLine("Current Spacing value: " + textOptions.Spacing);

            // Stelle neue Abstandswerte ein und sieh die Auswirkungen
            textOptions.Spacing = 2.0; // Increased spacing
            Console.WriteLine("Text with increased spacing (2.0)");

            // Speichere die Arbeitsmappe mit dem ersten Abstand
            workbook.Save("TextSpacingDemo1.xlsx");

            // Ändere den Abstand auf einen negativen Wert (Zeichen kommen näher zusammen)
            textOptions.Spacing = -1.0;
            Console.WriteLine("Text with decreased spacing (-1.0)");

            // Speichere die Arbeitsmappe mit dem zweiten Abstand
            workbook.Save("TextSpacingDemo2.xlsx");

            // Zurücksetzen auf den Standardabstand
            textOptions.Spacing = 0.0;
            Console.WriteLine("Text with default spacing (0.0)");

            // Speichere die Arbeitsmappe mit dem Standardabstand
            workbook.Save("TextSpacingDemo3.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


