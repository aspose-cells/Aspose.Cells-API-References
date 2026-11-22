---
title: "AutoNumberedBulletValue.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AutoNumberedBulletValue. تُرجع نوع الرصاصة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/autonumberedbulletvalue/type/
---
## AutoNumberedBulletValue.Type property

يحصل على نوع الرصاصة.

```csharp
public override BulletType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أنشئ شكلًا لإضافة نص مع الرصاصات
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 10, 300, 100);
            var textParagraph = shape.TextBody.TextParagraphs[0];

            // أنشئ قيمة رصاصة مرقمة تلقائيًا
            var bullet = new AutoNumberedBulletValue
            {
                AutonumberScheme = TextAutonumberScheme.AlphaLcParenBoth,
                StartAt = 1
            };

            // نظرًا لعدم إمكانية ضبط BulletValue مباشرةً، سنحتاج إلى إيجاد طريقة أخرى
            // لتطبيق نمط الرصاصة. قد يتطلب ذلك استخدام تنسيق نص الشكل
            // أو طرق أخرى متاحة في الـ API.
            // للتوضيح، سنعرض نوع الرصاصة فقط
            Console.WriteLine("Bullet Type: " + bullet.Type);

            // أضف نصًا إلى الفقرة عبر جسم نص الشكل
            shape.TextBody.Text = "First Item";

            // أضف فقرة أخرى بنظام ترقيم مختلف
            // نظرًا لأننا لا نستطيع الإضافة، سنستخدم الفقرة التالية المتاحة
            var secondParagraph = shape.TextBody.TextParagraphs[1];
            var bullet2 = new AutoNumberedBulletValue
            {
                AutonumberScheme = TextAutonumberScheme.Arabic1Minus,
                StartAt = 1
            };

            // اعرض نوع الرصاصة (خاصية للقراءة فقط)
            Console.WriteLine("Second Bullet Type: " + bullet2.Type);

            // أضف نصًا إلى الفقرة الثانية
            shape.TextBody.Text += "\nSecond Item";

            // احفظ المصنف لتوضيح تأثيرات التعداد
            workbook.Save("AutoNumberedBulletDemo.xlsx");
        }
    }

}
```

### انظر أيضًا

* enum [BulletType](../../bullettype/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


