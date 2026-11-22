---
title: "FontSettingCollection.TextParagraphs"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FontSettingCollection. تحصل على جميع الفقرات"
type: docs
url: /ar/net/aspose.cells.drawing.texts/fontsettingcollection/textparagraphs/
---
## FontSettingCollection.TextParagraphs property

يسترجع جميع الفقرات.

```csharp
public TextParagraphCollection TextParagraphs { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionPropertyTextParagraphsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف مربع نص إلى ورقة العمل
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "First paragraph\nSecond paragraph";

            // الوصول إلى الفقرة النصية الأولى
            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
            
            // تعيين خصائص تباعد الأسطر
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
            paragraph.LineSpace = 3000; // 300% line spacing

            // تعيين خصائص النقاط
            Bullet bullet = paragraph.Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // احفظ المصنف
            workbook.Save("TextParagraphsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextParagraphCollection](../../textparagraphcollection/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


