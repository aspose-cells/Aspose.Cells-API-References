---
title: "TextEffectFormat.Text"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextEffectFormat-Eigenschaft. Der Text im WordArt"
type: docs
url: /de/net/aspose.cells.drawing/texteffectformat/text/
---
## TextEffectFormat.Text property

Der Text im WordArt.

```csharp
public string Text { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyTextDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge eine Text-Effekt-Form hinzu und setze ihren Text
            Shape shape = sheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 14, false, false, 0, 0, 0, 0, 100, 100);

            // Greife auf die Text-Eigenschaft des Texteffekts zu und ändere sie
            shape.TextEffect.Text = "Updated Text";

            // Verifiziere, dass der Text aktualisiert wurde
            Console.WriteLine("Text Effect Content: " + shape.TextEffect.Text);
        }
    }
}
```

### Siehe auch

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


