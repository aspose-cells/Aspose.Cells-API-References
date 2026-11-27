---
title: "Klass Bullet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.Bullet klass. Representerar de punkter som ska tillämpas på ett stycke"
type: docs
url: /sv/net/aspose.cells.drawing.texts/bullet/
---
## Bullet class

Representerar att punktlistor ska tillämpas på ett stycke.

```csharp
public class Bullet
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BulletValue](../../aspose.cells.drawing.texts/bullet/bulletvalue/) { get; } | Hämtar värdet för bullet. |
| [FontName](../../aspose.cells.drawing.texts/bullet/fontname/) { get; set; } | Hämtar och anger namnet på teckensnittet. |
| [Type](../../aspose.cells.drawing.texts/bullet/type/) { get; set; } | Hämtar och anger typen av bullet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassBulletDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample text";

            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
            paragraph.LineSpace = 3000;

            Bullet bullet = paragraph.Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = 'v';
            bullet.FontName = "Arial";

            workbook.Save("TextsClassBulletDemo_Output.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


