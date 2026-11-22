---
title: "AutoNumberedBulletValue.AutonumberScheme"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AutoNumberedBulletValue. تمثل مخطط الرقم التلقائي"
type: docs
url: /ar/net/aspose.cells.drawing.texts/autonumberedbulletvalue/autonumberscheme/
---
## AutoNumberedBulletValue.AutonumberScheme property

تمثل مخطط الرقم التلقائي.

```csharp
public TextAutonumberScheme AutonumberScheme { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyAutonumberSchemeDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء نسخة جديدة من AutoNumberedBulletValue
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue();

                // اعرض القيمة الأولية لـ AutonumberScheme
                Console.WriteLine($"Default AutonumberScheme: {bullet.AutonumberScheme}");

                // عيّن قيمة جديدة لـ AutonumberScheme
                bullet.AutonumberScheme = TextAutonumberScheme.RomanUcPeriod;
                Console.WriteLine($"Modified AutonumberScheme: {bullet.AutonumberScheme}");

                // إنشاء مصنف لتوضيح التعداد في السياق
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // إنشاء شكل بنص سيستخدم نمط التعداد
                TextBox shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 100);
                shape.TextBody.Text = "Sample text with bullet formatting";


                // ملاحظة: تطبيق نمط التعداد الفعلي على النص سيتطلب استدعاءات API إضافية
                // غير معروض في الانعكاس. سنقوم فقط بحفظ المصنف كعرض توضيحي.
                workbook.Save("AutonumberSchemeDemo.xlsx");
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

* enum [TextAutonumberScheme](../../textautonumberscheme/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


