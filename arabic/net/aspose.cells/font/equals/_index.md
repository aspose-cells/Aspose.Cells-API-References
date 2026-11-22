---
title: "Font.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Font. تتحقق مما إذا كان الخطان متساويين"
type: docs
url: /ar/net/aspose.cells/font/equals/
---
## Font.Equals method

يتحقق مما إذا كان الخطان متساويين.

```csharp
public bool Equals(Font font)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خط | خط | كائن الخط المقارن. |

### قيمة الإرجاع

صحيح إذا كان مساويًا لكائن الخط المقارن.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontMethodEqualsWithFontDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء كائنين من الخط للمقارنة
            Font font1 = workbook.CreateStyle().Font;
            font1.Name = "Arial";
            font1.Size = 12;
            font1.IsBold = true;
            font1.Color = System.Drawing.Color.Black;

            Font font2 = workbook.CreateStyle().Font;
            font2.Name = "Arial";
            font2.Size = 12;
            font2.IsBold = true;
            font2.Color = System.Drawing.Color.Black;

            try
            {
                // استدعاء طريقة Equals لمقارنة الخطوط
                bool areEqual = font1.Equals(font2);

                // اعرض النتيجة
                Console.WriteLine($"The fonts are equal: {areEqual}");

                // تعديل أحد الخطوط لجعله مختلفًا
                font2.IsItalic = true;
                areEqual = font1.Equals(font2);
                Console.WriteLine($"After modification, the fonts are equal: {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("FontEqualsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


