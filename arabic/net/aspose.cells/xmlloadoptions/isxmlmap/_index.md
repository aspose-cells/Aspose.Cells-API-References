---
title: "XmlLoadOptions.IsXmlMap"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XmlLoadOptions. تشير إلى ما إذا كان يتم ربط XML بـ Excel. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/xmlloadoptions/isxmlmap/
---
## XmlLoadOptions.IsXmlMap property

يشير إلى ما إذا كان يتم تحويل XML إلى Excel. القيمة الافتراضية هي false.

```csharp
public bool IsXmlMap { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyIsXmlMapDemo
    {
        public static void Run()
        {
            // إنشاء مثيل من XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // تمكين ربط XML عند تحميل الملف
            options.IsXmlMap = true;

            // تحميل ملف XML إلى مصنف باستخدام الخيارات المحددة
            Workbook workbook = new Workbook("sample.xml", options);

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // عرض بعض البيانات من XML المحمّل لتوضيح نجاح الربط
            Console.WriteLine("Data from loaded XML:");
            Console.WriteLine(worksheet.Cells["A1"].StringValue);
            Console.WriteLine(worksheet.Cells["A2"].StringValue);

            // حفظ المصنف إلى ملف Excel جديد
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


