---
title: "XmlLoadOptions.IgnoreRootAttributes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XmlLoadOptions. تشير إلى ما إذا كان يتم تجاهل سمات العنصر الجذر"
type: docs
url: /ar/net/aspose.cells/xmlloadoptions/ignorerootattributes/
---
## XmlLoadOptions.IgnoreRootAttributes property

يشير إلى ما إذا كان يتم تجاهل سمات العنصر الجذر.

```csharp
public bool IgnoreRootAttributes { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyIgnoreRootAttributesDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل XML وتعيين IgnoreRootAttributes
            XmlLoadOptions options = new XmlLoadOptions();
            options.IgnoreRootAttributes = true;

            // تحميل ملف XML باستخدام الخيارات
            Workbook workbook = new Workbook("example.xml", options);

            // الوصول إلى البيانات من XML المحمّل
            string cellValue = workbook.Worksheets[0].Cells["AH8"].StringValue;
            Console.WriteLine("Cell AH8 value: " + cellValue);

            // حفظ كـ XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


