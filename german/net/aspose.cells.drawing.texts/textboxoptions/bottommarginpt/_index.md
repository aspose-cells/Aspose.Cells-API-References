---
title: "TextBoxOptions.BottomMarginPt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxOptions-Eigenschaft. Gibt den unteren Rand in der Einheit Punkte zurück."
type: docs
url: /de/net/aspose.cells.drawing.texts/textboxoptions/bottommarginpt/
---
## TextBoxOptions.BottomMarginPt property

Gibt den unteren Rand in Punkten zurück

```csharp
public double BottomMarginPt { get; set; }
```

### Beispiele

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

### Siehe auch

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


