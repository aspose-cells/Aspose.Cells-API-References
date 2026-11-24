---
title: "Shape.GetRichFormattings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Text darstellen."
type: docs
url: /de/net/aspose.cells.drawing/shape/getrichformattings/
---
## Shape.GetRichFormattings method

Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Text darstellen.

```csharp
public FontSetting[] GetRichFormattings()
```

### Rückgabewert

Alle Characters-Objekte

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Form mit Rich-Text hinzufügen (korrekte Parameteranzahl für AddRectangle)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "This is bold and this is italic";
            
            // Teile des Textes formatieren
            shape.Characters(0, 4).Font.IsBold = true;
            shape.Characters(13, 6).Font.IsItalic = true;

            // Rufe Rich‑Text‑Formatierungen ab
            FontSetting[] formattings = shape.GetRichFormattings();

            // Zeige Formatierungsinformationen an
            Console.WriteLine("Rich text formattings:");
            foreach (FontSetting setting in formattings)
            {
                Console.WriteLine($"Text segment: '{shape.Text.Substring(setting.StartIndex, setting.Length)}'");
                Console.WriteLine($"Start index: {setting.StartIndex}");
                Console.WriteLine($"Length: {setting.Length}");
                Console.WriteLine($"Bold: {setting.Font.IsBold}");
                Console.WriteLine($"Italic: {setting.Font.IsItalic}");
                Console.WriteLine();
            }
        }
    }
}
```

### Siehe auch

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


