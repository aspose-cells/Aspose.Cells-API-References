---
title: "الفئة NoneBulletValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.Texts.NoneBulletValue فئة. تمثل عدم وجود نقطة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/nonebulletvalue/
---
## NoneBulletValue class

يمثل عدم وجود رصاصة.

```csharp
public class NoneBulletValue : BulletValue
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [NoneBulletValue](nonebulletvalue/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| override [Type](../../aspose.cells.drawing.texts/nonebulletvalue/type/) { get; } | يحصل على نوع قيمة النقطة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class NoneBulletValueDemo
    {
        public static void NoneBulletValueExample()
        {
            // إنشاء مصنف جديد والوصول إلى ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة نص إلى خلية
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample text without bullet");

            // إنشاء TextBox لتطبيق إعدادات النقطة
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[worksheet.TextBoxes.Add(2, 1, 100, 400)];
            textBox.Text = "This is a TextBox without bullet points";

            // إنشاء نسخة من NoneBulletValue
            NoneBulletValue noneBulletValue = new NoneBulletValue();

            // تحقق من نوع النقطة (يجب أن تكون None)
            BulletType bulletType = noneBulletValue.Type;
            Console.WriteLine("Bullet Type: " + bulletType); // Output should be None

            // حفظ المصنف لتوضيح التغييرات
            workbook.Save("NoneBulletValueExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


