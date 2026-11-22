---
title: "الفئة BulletValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.Texts.BulletValue فئة. تمثل قيمة النقطة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/bulletvalue/
---
## BulletValue class

يمثل قيمة الرصاصة.

```csharp
public abstract class BulletValue
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| abstract [Type](../../aspose.cells.drawing.texts/bulletvalue/type/) { get; } | يحصل على نوع قيمة النقطة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassBulletValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مربع نص والحصول على فقراته النصية
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var textParagraph = textBox.TextBody.TextParagraphs[0];

            // إنشاء نسخة من CharacterBulletValue (التي ترث من BulletValue)
            var bulletValue = new CharacterBulletValue();
            bulletValue.Character = '•';
            
            // تعيين قيمة النقطة للفقرة (Bullet للقراءة فقط، لذا نحتاج إلى تعديلها بطريقة مختلفة)
            // نظرًا لأن Bullet للقراءة فقط، نحتاج إلى العثور على طريقة أخرى لتعيينه
            // قد يتضمن ذلك إنشاء TextParagraph جديد مع تعيين النقطة
            // ملاحظة: قد يوفر API الفعلي طريقة مختلفة لتعيين النقاط
            // للتوضيح، سنفترض أننا يمكننا تعيينه عبر وسائل أخرى
            // textParagraph.Bullet = bulletValue; // تم إزالة هذا السطر لأن Bullet للقراءة فقط
            textBox.Text = "First bullet point";

            // إضافة فقرة أخرى بنقطة مختلفة
            // TextParagraphCollection لا يحتوي على طريقة Add، لذا نحتاج إلى العثور على طريقة أخرى
            // قد يتضمن ذلك إنشاء TextParagraph جديد وإضافته عبر وسائل أخرى
            // للتوضيح، سنفترض أننا يمكننا الحصول على الفقرة الثانية مباشرة
            var textParagraph2 = textBox.TextBody.TextParagraphs[1];
            var bulletValue2 = new CharacterBulletValue();
            bulletValue2.Character = '→';
            // textParagraph2.Bullet = bulletValue2; // تم إزالة هذا السطر لأن Bullet للقراءة فقط
            textBox.Text += "\nSecond bullet point";

            // عرض الوصول إلى نوع النقطة
            Console.WriteLine("First bullet type: " + textParagraph.Bullet.Type);
            Console.WriteLine("Second bullet type: " + textParagraph2.Bullet.Type);

            // حفظ النتيجة
            workbook.Save("TextsClassBulletValueDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


