---
title: "HtmlSaveOptions.EncodeEntityAsCode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. توضح ما إذا كانت كيانات الأحرف html تُستبدل برمز عشري. على سبيل المثال، يتم استبدال nbsp بـ 160. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/encodeentityascode/
---
## HtmlSaveOptions.EncodeEntityAsCode property

يشير إلى ما إذا كانت كيانات أحرف html تُستبدل بالرمز العشري. (مثال: "&amp;nbsp;" تُستبدل بـ "&amp;#160;"). القيمة الافتراضية هي false.

```csharp
public bool EncodeEntityAsCode { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class HtmlSaveOptionsPropertyEncodeEntityAsCodeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية مع أحرف خاصة
            worksheet.Cells["A1"].PutValue("Sample & Text");
            worksheet.Cells["A2"].PutValue("Another <Test> String");
            worksheet.Cells["A3"].PutValue("Price: $100");

            // إنشاء خيارات حفظ HTML
            HtmlSaveOptions options = new HtmlSaveOptions();

            // عرض القيمة الحالية لـ EncodeEntityAsCode
            Console.WriteLine("Current EncodeEntityAsCode value: " + options.EncodeEntityAsCode);

            // تعيين EncodeEntityAsCode إلى true
            options.EncodeEntityAsCode = true;

            // حفظ مع تشفير الكيانات كرمز
            workbook.Save("HtmlWithEncodedEntities.html", options);

            // تعيين EncodeEntityAsCode إلى false
            options.EncodeEntityAsCode = false;

            // حفظ الكيانات كما هي
            workbook.Save("HtmlWithRawEntities.html", options);

            // مقارنة ملفات الإخراج
            Console.WriteLine("Files created:");
            Console.WriteLine("1. HtmlWithEncodedEntities.html - with encoded entities");
            Console.WriteLine("2. HtmlWithRawEntities.html - with raw entities");
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


