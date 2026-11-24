---
title: "TextOptions.Kerning"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextOptions-Eigenschaft. Gibt die minimale Schriftgröße an, bei der Zeichenkerning für diesen Textlauf erfolgt"
type: docs
url: /de/net/aspose.cells.drawing.texts/textoptions/kerning/
---
## TextOptions.Kerning property

Gibt die minimale Schriftgröße an, bei der für diesen Textlauf Kerning zwischen Zeichen erfolgt.

```csharp
public double Kerning { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyKerningDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form mit Text hinzu, um Kerning zu demonstrieren
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
            shape.Text = "Kerning Demonstration Text";

            // Rufe die TextOptions der Form ab
            TextOptions textOptions = shape.TextOptions;

            // Zeige den aktuellen Kerning-Wert an
            Console.WriteLine("Current Kerning value: " + textOptions.Kerning);

            // Kerning auf 12 Punkte einstellen (Mindestschriftgröße, damit Kerning angewendet wird)
            textOptions.Kerning = 12;

            // Eine größere Schriftgröße einstellen, um den Kerning-Effekt zu beobachten
            textOptions.Size = 24;

            // Speichern Sie die Arbeitsmappe, um den Effekt zu sehen
            workbook.Save("PropertyKerningDemo.xlsx");

            // Erstelle eine weitere Form mit unterschiedlichem Kerning zum Vergleich
            var shape2 = worksheet.Shapes.AddTextBox(10, 0, 1, 0, 200, 100);
            shape2.Text = "Comparison Text Without Kerning";
            shape2.TextOptions.Size = 24;
            shape2.TextOptions.Kerning = 0; // No kerning

            // Erneut speichern mit beiden Beispielen
            workbook.Save("PropertyKerningDemoWithComparison.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


