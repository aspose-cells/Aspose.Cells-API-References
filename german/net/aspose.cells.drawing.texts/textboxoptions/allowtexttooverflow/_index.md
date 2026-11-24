---
title: "TextBoxOptions.AllowTextToOverflow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxOptions-Eigenschaft. Gibt an, ob Text das Formfeld überlaufen darf."
type: docs
url: /de/net/aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/
---
## TextBoxOptions.AllowTextToOverflow property

Ob Text die Form überlaufen darf.

```csharp
public bool AllowTextToOverflow { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyAllowTextToOverflowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // Setze Text, der möglicherweise überläuft
            textBox.Text = "This is a long text that might overflow the text box boundaries if AllowTextToOverflow is false";

            // Aktiviere Textüberlauf
            textBox.TextBoxOptions.AllowTextToOverflow = true;

            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxAllowTextToOverflowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


