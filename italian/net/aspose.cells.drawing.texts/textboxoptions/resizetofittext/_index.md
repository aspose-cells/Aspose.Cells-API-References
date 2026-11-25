---
title: "TextBoxOptions.ResizeToFitText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxOptions. Indica se ridimensionare la forma per adattare il testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textboxoptions/resizetofittext/
---
## TextBoxOptions.ResizeToFitText property

Indica se ridimensionare la forma per adattarla al testo

```csharp
public bool ResizeToFitText { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyResizeToFitTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una casella di testo con i parametri corretti
            Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(1, 1, 100, 100, 200, 50);
            textBox.Text = "This is a sample text that will make the text box resize to fit";

            // Accedi a TextBoxOptions correttamente
            textBox.TextBoxOptions.ResizeToFitText = true;

            // Salva la cartella di lavoro
            workbook.Save("TextBoxResizeToFitTextDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


