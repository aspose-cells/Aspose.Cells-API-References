---
title: "TextBoxOptions.AllowTextToOverflow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxOptions. Se consentire al testo di traboccare dalla forma"
type: docs
url: /it/net/aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/
---
## TextBoxOptions.AllowTextToOverflow property

Se consentire al testo di traboccare dalla forma.

```csharp
public bool AllowTextToOverflow { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // Imposta il testo che potrebbe traboccare
            textBox.Text = "This is a long text that might overflow the text box boundaries if AllowTextToOverflow is false";

            // Abilita il trabocco del testo
            textBox.TextBoxOptions.AllowTextToOverflow = true;

            // Salva la cartella di lavoro
            workbook.Save("TextBoxAllowTextToOverflowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


