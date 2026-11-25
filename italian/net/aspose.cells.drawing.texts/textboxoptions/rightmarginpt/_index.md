---
title: "TextBoxOptions.RightMarginPt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxOptions. Ottiene e imposta il margine destro in unità di punti"
type: docs
url: /it/net/aspose.cells.drawing.texts/textboxoptions/rightmarginpt/
---
## TextBoxOptions.RightMarginPt property

Ottiene e imposta il margine destro in unità di Punti.

```csharp
public double RightMarginPt { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyRightMarginPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            int textBoxIndex = worksheet.TextBoxes.Add(1, 1, 200, 200);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "Sample Text";

            // Imposta il margine destro in punti
            textBox.TextBoxOptions.RightMarginPt = 0.2d;

            // Salva la cartella di lavoro
            workbook.Save("TextBoxRightMarginDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


