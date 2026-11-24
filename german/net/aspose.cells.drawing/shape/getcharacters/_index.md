---
title: "Shape.GetCharacters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Text darstellen."
type: docs
url: /de/net/aspose.cells.drawing/shape/getcharacters/
---
## Shape.GetCharacters method

Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Text darstellen.

```csharp
[Obsolete("Use Shape.GetRichFormattings() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetCharacters()
```

### Rückgabewert

Alle Characters-Objekte

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode Shape.GetRichFormattings(). Diese Methode wird 12 Monate nach November 2023 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetCharactersDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein Textfeld-Shape zum Arbeitsblatt mit allen erforderlichen Parametern hinzu
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            shape.Text = "Sample Text";

            // Holen Sie die Zeichen aus dem Shape
            ArrayList characters = shape.GetCharacters();

            // Zeigen Sie Informationen zu jedem Zeichen an
            foreach (FontSetting charSetting in characters)
            {
                Console.WriteLine($"Font: {charSetting.Font.Name}, Size: {charSetting.Font.Size}");
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


