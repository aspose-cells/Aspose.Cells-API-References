---
title: "الفئة Bullet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.Texts.Bullet. تمثل نقاط التعداد التي يجب تطبيقها على فقرة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/bullet/
---
## Bullet class

يمثل bullet points التي يجب تطبيقها على فقرة.

```csharp
public class Bullet
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BulletValue](../../aspose.cells.drawing.texts/bullet/bulletvalue/) { get; } | يحصل على قيمة bullet. |
| [FontName](../../aspose.cells.drawing.texts/bullet/fontname/) { get; set; } | يحصل على اسم الخط ويضبطه. |
| [Type](../../aspose.cells.drawing.texts/bullet/type/) { get; set; } | يحصل على نوع bullet ويضبطه. |

### أمثلة

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

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


