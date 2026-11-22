---
title: "FontSetting.Length"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FontSetting. تحصل على طول الأحرف"
type: docs
url: /ar/net/aspose.cells/fontsetting/length/
---
## FontSetting.Length property

يحصل على طول الأحرف.

```csharp
public int Length { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingPropertyLengthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل والوصول إلى ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض النص إلى الخلية A1
            worksheet.Cells["A1"].PutValue("Hello World");

            // إنشاء إعدادات الخط للنص في الخلية A1
            FontSetting fontSetting = worksheet.Cells["A1"].Characters(0, 5);
            
            // عرض استخدام خاصية Length
            Console.WriteLine("Original Length: " + fontSetting.Length);
            
            // تعديل طول إعداد الخط
            fontSetting = worksheet.Cells["A1"].Characters(0, 11);
            Console.WriteLine("Modified Length: " + fontSetting.Length);
            
            // تطبيق التنسيق على إعداد الخط
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            
            // احفظ المصنف
            workbook.Save("FontSettingLengthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


