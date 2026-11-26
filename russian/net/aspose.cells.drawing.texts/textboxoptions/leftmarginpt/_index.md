---
title: "TextBoxOptions.LeftMarginPt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextBoxOptions. Получает и задает левый отступ в единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textboxoptions/leftmarginpt/
---
## TextBoxOptions.LeftMarginPt property

Получает и задает левый отступ в единицах точек.

```csharp
public double LeftMarginPt { get; set; }
```

### Примеры

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

### См. также

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


