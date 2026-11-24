---
title: "TextBoxOptions.WrapTextInShape"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxOptions-Eigenschaft. Gibt an, ob Text in einer Form umbrochen wird. False  Es wird kein Umbruch im Textkörper stattfinden. True  Der Textkörper wird umbrochen"
type: docs
url: /de/net/aspose.cells.drawing.texts/textboxoptions/wraptextinshape/
---
## TextBoxOptions.WrapTextInShape property

Gibt an, wie der Text in einer Form umbrochen wird. False - Es erfolgt kein Umbruch im Textkörper. True - Es erfolgt ein Umbruch im Textkörper.

```csharp
public bool WrapTextInShape { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyWrapTextInShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Textfeld-Form mit korrekten Parametern hinzu
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);

            // Setze Text, der innerhalb der Form umbrochen wird
            textBox.Text = "This is a long text that should wrap within the text box shape boundaries when WrapTextInShape is enabled.";

            // Aktiviere Textumbruch innerhalb der Form
            textBox.TextBoxOptions.WrapTextInShape = true;

            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxWrapTextDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


