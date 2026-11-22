---
title: "HtmlSaveOptions.WidthScalable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "HtmlSaveOptions property. يشير إلى ما إذا كان يتم تصدير عرض العمود بوحدة المقياس إلى html. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/widthscalable/
---
## HtmlSaveOptions.WidthScalable property

يشير إلى ما إذا كان يتم تصدير عرض العمود بوحدة المقياس إلى HTML. القيمة الافتراضية هي false.

```csharp
public bool WidthScalable { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyWidthScalableDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل تجريبي مع بيانات اختبار
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test WidthScalable Property");
            worksheet.Cells["B1"].PutValue(123.45);
            
            // حدد خيارات حفظ HTML باستخدام الخاصية WidthScalable
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.WidthScalable = true; // Demonstrate setting to true
            
            // احفظ بعرض قابل للتوسيع
            workbook.Save("output_scalable.html", options);
            
            // احفظ مرة أخرى بعرض ثابت
            options.WidthScalable = false;
            workbook.Save("output_fixed.html", options);
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


