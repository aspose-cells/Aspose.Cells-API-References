---
title: "Enum LineSpaceSizeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.LineSpaceSizeType enum. Representerar enhetstypen för radavståndsstorlek"
type: docs
url: /sv/net/aspose.cells.drawing.texts/linespacesizetype/
---
## LineSpaceSizeType enumeration

Representerar enhetstypen för radavståndsstorlek.

```csharp
public enum LineSpaceSizeType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Percentage | `0` | Representerar en enhet i procent av textstorleken. |
| Points | `1` | Representerar i enhet av punkter. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassLineSpaceSizeTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en textruta
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Ange textinnehåll
            textBox.Text = "Sample Text\nSecond Line";
            
            // Få åtkomst till det första stycket i textrutan
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];
            
            // Ställ in storlekstyp för efteravstånd till punkter
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            
            // Ställ in efteravståndsvärde (12 punkter)
            paragraph.SpaceAfter = 12;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Text box with line spacing created successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


