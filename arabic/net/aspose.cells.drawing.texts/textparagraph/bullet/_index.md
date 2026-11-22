---
title: "TextParagraph.Bullet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextParagraph. تحصل على النقطة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textparagraph/bullet/
---
## TextParagraph.Bullet property

الحصول على الرصاصة.

```csharp
public Bullet Bullet { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertyBulletDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف مربع نص
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            
            // اضبط النص وقم بتكوين الفقرة
            textbox.Text = "First Item\nSecond Item";
            textbox.TextBody.TextParagraphs[0].LineSpaceSizeType = LineSpaceSizeType.Percentage;
            textbox.TextBody.TextParagraphs[0].LineSpace = 3000;

            // قم بتكوين النقطة للفقرة الأولى
            Bullet bullet = textbox.TextBody.TextParagraphs[0].Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // احفظ المصنف
            workbook.Save("TextParagraphPropertyBulletDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Bullet](../../bullet/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


