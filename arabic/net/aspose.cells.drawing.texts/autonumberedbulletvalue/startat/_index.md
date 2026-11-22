---
title: "AutoNumberedBulletValue.StartAt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AutoNumberedBulletValue. تُرجع وتضبط الرقم الابتدائي للترقيم"
type: docs
url: /ar/net/aspose.cells.drawing.texts/autonumberedbulletvalue/startat/
---
## AutoNumberedBulletValue.StartAt property

يحصل ويضبط الرقم الابتدائي للرصاصة.

```csharp
public int StartAt { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyStartAtDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // إنشاء مثيل AutoNumberedBulletValue
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue
                {
                    AutonumberScheme = TextAutonumberScheme.ArabicPeriod,
                    StartAt = 3 // Setting the StartAt property
                };

                // اعرض القيمة الحالية لـ StartAt
                Console.WriteLine($"Initial StartAt value: {bullet.StartAt}");

                // عدّل قيمة StartAt
                bullet.StartAt = 5;
                Console.WriteLine($"Modified StartAt value: {bullet.StartAt}");

                // أنشئ شكلًا لتوضيح الرصاصة في السياق
                var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 100);
                shape.TextBody.Text = "1. First Item\n2. Second Item";

                // تطبيق نمط الرصاصة (ملاحظة: طريقة التطبيق الفعلية غير معروضة في الانعكاس)
                // للتوضيح، سنقوم بحفظ المصنف فقط
                workbook.Save("StartAtPropertyDemo.xlsx");
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

* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


