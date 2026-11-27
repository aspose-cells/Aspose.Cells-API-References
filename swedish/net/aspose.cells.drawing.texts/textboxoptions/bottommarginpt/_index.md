---
title: "TextBoxOptions.BottomMarginPt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxOptions-egenskap. Returnerar bottenmarginalen i enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textboxoptions/bottommarginpt/
---
## TextBoxOptions.BottomMarginPt property

Returnerar den nedre marginalen i enheten punkter

```csharp
public double BottomMarginPt { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyBottomMarginPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            shape.TextBoxOptions.BottomMarginPt = 0.2d;

            Console.WriteLine("Bottom margin set to: " + shape.TextBoxOptions.BottomMarginPt + " points");
        }
    }
}
```

### Se även

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


