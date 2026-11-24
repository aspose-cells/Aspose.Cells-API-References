---
title: "TextOptions.LatinName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextOptions-Eigenschaft. Liest und setzt den lateinischen Namen"
type: docs
url: /de/net/aspose.cells.drawing.texts/textoptions/latinname/
---
## TextOptions.LatinName property

Liest und setzt den lateinischen Namen.

```csharp
public string LatinName { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyLatinNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um Textoptionen zu demonstrieren
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            shape.Text = "Sample Text";

            // Rufe die TextOptions aus dem ersten Absatz der Form ab
            TextOptions textOptions = shape.TextBody.TextParagraphs[0].TextOptions;

            // Zeige den aktuellen LatinName-Wert an
            Console.WriteLine("Current LatinName value: " + textOptions.LatinName);

            // Setze einen neuen LatinName-Wert
            textOptions.LatinName = "Times New Roman";

            // Erstelle eine weitere Form, um die Schriftartdarstellung zu vergleichen
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 0, 3, 0, 100, 150);
            shape2.Text = "Comparison Text";
            shape2.TextBody.TextParagraphs[0].TextOptions.LatinName = "Arial";

            // Speichere die Arbeitsmappe, um die Auswirkungen zu sehen
            workbook.Save("PropertyLatinNameDemo.xlsx");

            // Zeige den neuen LatinName-Wert an
            Console.WriteLine("New LatinName value: " + textOptions.LatinName);
        }
    }
}
```

### Siehe auch

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


