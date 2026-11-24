---
title: "TextOptions.UnderlineColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextOptions-Eigenschaft. Liest oder setzt die Farbe der Unterstreichung"
type: docs
url: /de/net/aspose.cells.drawing.texts/textoptions/underlinecolor/
---
## TextOptions.UnderlineColor property

Liest oder setzt die Farbe der Unterstreichung.

```csharp
public CellsColor UnderlineColor { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyUnderlineColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form mit Text hinzu, um Textoptionen zu demonstrieren
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
            shape.Text = "Underline Color Demo";
            
            // Erhalte die TextOptions aus der Form
            TextOptions textOptions = shape.TextOptions;

            try
            {
                // Zeige den aktuellen UnderlineColor-Wert an
                CellsColor currentColor = textOptions.UnderlineColor;
                Console.WriteLine($"Current UnderlineColor - Type: {currentColor.Type}, Color: {currentColor.Color}");

                // Setze ein neues UnderlineColor (da die Eigenschaft lesbar und schreibbar ist)
                CellsColor newColor = textOptions.UnderlineColor; // Use existing color object
                newColor.Color = System.Drawing.Color.Red;
                textOptions.UnderlineColor = newColor;

                // Aktiviere Unterstreichung, um den Effekt zu sehen
                textOptions.Underline = FontUnderlineType.Single;

                // Zeige den neuen UnderlineColor-Wert an
                Console.WriteLine($"New UnderlineColor - Type: {textOptions.UnderlineColor.Type}, Color: {textOptions.UnderlineColor.Color}");

                // Speichern Sie die Arbeitsmappe, um den Effekt zu sehen
                workbook.Save("UnderlineColorDemo.xlsx");
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


