---
title: "TextBoxOptions.WrapTextInShape"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxOptions. Specifica l'andare a capo del testo all'interno di una forma. False Nessun a capo avverrà sul corpo del testo. True L'andare a capo avverrà sul corpo del testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textboxoptions/wraptextinshape/
---
## TextBoxOptions.WrapTextInShape property

Specifica l'adattamento del testo all'interno di una forma. False - Nessun adattamento avverrà sul corpo del testo. True - L'adattamento avverrà sul corpo del testo.

```csharp
public bool WrapTextInShape { get; set; }
```

### Esempi

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

            // Aggiungi una forma casella di testo con i parametri corretti
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);

            // Imposta il testo che andrà a capo all'interno della forma
            textBox.Text = "This is a long text that should wrap within the text box shape boundaries when WrapTextInShape is enabled.";

            // Abilita l'andare a capo del testo all'interno della forma
            textBox.TextBoxOptions.WrapTextInShape = true;

            // Salva la cartella di lavoro
            workbook.Save("TextBoxWrapTextDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


