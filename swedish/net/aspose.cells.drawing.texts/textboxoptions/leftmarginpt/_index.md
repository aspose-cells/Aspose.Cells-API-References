---
title: "TextBoxOptions.LeftMarginPt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxOptions egenskap. Hämtar och anger vänstermarginalen i enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textboxoptions/leftmarginpt/
---
## TextBoxOptions.LeftMarginPt property

Hämtar och anger den vänstra marginalen i enheten punkter.

```csharp
public double LeftMarginPt { get; set; }
```

### Exempel

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

### Se även

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


