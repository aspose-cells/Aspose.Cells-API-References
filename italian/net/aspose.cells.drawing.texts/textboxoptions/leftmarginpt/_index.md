---
title: "TextBoxOptions.LeftMarginPt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxOptions. Ottiene e imposta il margine sinistro in unità di punti"
type: docs
url: /it/net/aspose.cells.drawing.texts/textboxoptions/leftmarginpt/
---
## TextBoxOptions.LeftMarginPt property

Ottiene e imposta il margine sinistro in unità di Punti.

```csharp
public double LeftMarginPt { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyLeftMarginPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 400);
            textBox.TextBoxOptions.LeftMarginPt = 0.2d;

            Console.WriteLine("Left margin set to: " + textBox.TextBoxOptions.LeftMarginPt + " points");
        }
    }
}
```

### Vedi anche

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


