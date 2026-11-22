---
title: "BulletValue.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BulletValue. تحصل على نوع قيمة الرصاصات"
type: docs
url: /ar/net/aspose.cells.drawing.texts/bulletvalue/type/
---
## BulletValue.Type property

يحصل على نوع قيمة النقطة.

```csharp
public abstract BulletType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class BulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء مربع نص والحصول على فقراته النصية
                var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
                var textParagraph = textBox.TextBody.TextParagraphs[0];

                // إنشاء قيمة رصاص حرفية (التي ترث من BulletValue)
                var bulletValue = new CharacterBulletValue();
                bulletValue.Character = '•';

                // عرض قيمة خاصية Type
                Console.WriteLine("Bullet Type: " + bulletValue.Type);

                // إنشاء قيمة رصاص صورة لعرض نوع مختلف
                var pictureBullet = new PictureBulletValue();
                Console.WriteLine("Picture Bullet Type: " + pictureBullet.Type);

                // احفظ المصنف
                workbook.Save("BulletValueTypeDemo.xlsx");
                Console.WriteLine("Type property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [BulletType](../../bullettype/)
* class [BulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


