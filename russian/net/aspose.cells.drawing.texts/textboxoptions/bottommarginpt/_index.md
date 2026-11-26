---
title: "TextBoxOptions.BottomMarginPt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "TextBoxOptions property. Возвращает нижний отступ в единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textboxoptions/bottommarginpt/
---
## TextBoxOptions.BottomMarginPt property

Возвращает нижний отступ в единицах Points

```csharp
public double BottomMarginPt { get; set; }
```

### Примеры

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

### См. также

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


