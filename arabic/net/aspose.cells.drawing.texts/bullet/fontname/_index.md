---
title: "Bullet.FontName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Bullet. تحصل وتعيّن اسم الخط"
type: docs
url: /ar/net/aspose.cells.drawing.texts/bullet/fontname/
---
## Bullet.FontName property

يحصل على اسم الخط ويضبطه.

```csharp
public string FontName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class BulletPropertyFontNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample text with bullet";

            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
            paragraph.LineSpace = 3000;

            Bullet bullet = paragraph.Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            workbook.Save("BulletFontNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Bullet](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


