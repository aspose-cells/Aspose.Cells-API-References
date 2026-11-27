---
title: "TextBoxOptions.RightMarginPt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxOptions-egenskap. Hämtar och anger högermarginalen i enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textboxoptions/rightmarginpt/
---
## TextBoxOptions.RightMarginPt property

Hämtar och anger den högra marginalen i enheten punkter.

```csharp
public double RightMarginPt { get; set; }
```

### Exempel

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

            // Lägg till en textruta i kalkylbladet
            int textBoxIndex = worksheet.TextBoxes.Add(1, 1, 200, 200);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "Sample Text";

            // Ange högermarginalen i punkter
            textBox.TextBoxOptions.RightMarginPt = 0.2d;

            // Spara arbetsboken
            workbook.Save("TextBoxRightMarginDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


