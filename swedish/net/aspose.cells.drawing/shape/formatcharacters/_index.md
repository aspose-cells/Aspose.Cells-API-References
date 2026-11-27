---
title: "Shape.FormatCharacters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-metod. Formaterar vissa tecken med teckensnittsinställningen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/formatcharacters/
---
## Shape.FormatCharacters method

Formaterar vissa tecken med teckensnittsinställningen.

```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | Int32 | Startindexet. |
| length | Int32 | Längden. |
| teckensnitt | Teckensnitt | Teckensnittinställningen. |
| flagga | StyleFlag | Flaggan för teckensnittsinställningen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodFormatCharactersWithInt32Int32FontStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en textruta i kalkylbladet
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            textBox.Text = "Sample Text Formatting";
            
            // Skapa ett teckensnitt med önskade egenskaper
            Aspose.Cells.Font font = textBox.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            
            // Skapa stilflagga för att ange vilka egenskaper som ska tillämpas
            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontBold = true;
            
            // Applicera formatering på specifika tecken
            textBox.FormatCharacters(0, 6, font, flag);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


