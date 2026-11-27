---
title: "TextBoxOptions.WrapTextInShape"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxOptions-egenskap. Anger textbrytning inom en form. False  Ingen brytning kommer att ske i textkroppen. True  Brytning kommer att ske i textkroppen"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textboxoptions/wraptextinshape/
---
## TextBoxOptions.WrapTextInShape property

Anger textbrytning inom en form. Falskt - Ingen brytning sker i textområdet. Sant - Brytning sker i textområdet.

```csharp
public bool WrapTextInShape { get; set; }
```

### Exempel

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

            // Lägg till en textrutaform med korrekta parametrar
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);

            // Ange text som ska brytas inom formen
            textBox.Text = "This is a long text that should wrap within the text box shape boundaries when WrapTextInShape is enabled.";

            // Aktivera textbrytning inom formen
            textBox.TextBoxOptions.WrapTextInShape = true;

            // Spara arbetsboken
            workbook.Save("TextBoxWrapTextDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


