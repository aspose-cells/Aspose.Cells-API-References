---
title: "XmlLoadOptions.NumberFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XmlLoadOptions. تحصل وتضبط تنسيق القيمة الرقمية"
type: docs
url: /ar/net/aspose.cells/xmlloadoptions/numberformat/
---
## XmlLoadOptions.NumberFormat property

يحصل ويضبط تنسيق القيمة الرقمية.

```csharp
public string NumberFormat { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // إنشاء مثيل من XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // تعيين خاصية NumberFormat لعرض الأعداد بدقة منزلتين عشريتين
            options.NumberFormat = "0.00";

            // تحميل ملف XML إلى مصنف باستخدام الخيارات المحددة
            Workbook workbook = new Workbook("input.xml", options);

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين بعض القيم الرقمية لتوضيح تنسيق الأعداد
            worksheet.Cells["A1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(45.678);
            worksheet.Cells["A3"].PutValue(0.5);

            // حفظ دفتر العمل إلى ملف جديد
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


