---
title: "XmlLoadOptions.DateFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XmlLoadOptions. تحصل وتضبط تنسيق قيمة التاريخ"
type: docs
url: /ar/net/aspose.cells/xmlloadoptions/dateformat/
---
## XmlLoadOptions.DateFormat property

يحصل على ويضبط تنسيق قيمة التاريخ.

```csharp
public string DateFormat { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // إنشاء مثيل من XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // تعيين تنسيق التاريخ لتحليل التواريخ من XML
            options.DateFormat = "yyyy-MM-dd";
            options.ConvertNumericOrDate = true;

            // تحميل ملف XML إلى مصنف باستخدام الخيارات المحددة
            Workbook workbook = new Workbook("input.xml", options);

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // عرض بعض الخلايا لتوضيح تنسيق التاريخ
            Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].Value);

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


