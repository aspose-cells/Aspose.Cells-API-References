---
title: "TextBoxOptions.TopMarginPt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxOptions-egenskap. Hämtar och anger topmargin i enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textboxoptions/topmarginpt/
---
## TextBoxOptions.TopMarginPt property

Hämtar och anger den övre marginalen i enheten punkter.

```csharp
public double TopMarginPt { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyTopMarginPtDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en textruta i kalkylbladet
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Ange topmargin i punkter
            textBox.TextBoxOptions.TopMarginPt = 0.2d;
            
            // Spara arbetsboken
            workbook.Save("TextBoxTopMarginDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


