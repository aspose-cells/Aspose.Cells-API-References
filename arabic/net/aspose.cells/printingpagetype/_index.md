---
title: "تعداد PrintingPageType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.PrintingPageType. يوضح أي الصفحات لن تُطبع"
type: docs
url: /ar/net/aspose.cells/printingpagetype/
---
## PrintingPageType enumeration

يشير إلى الصفحات التي لن تُطبع.

```csharp
public enum PrintingPageType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Default | `0` | يطبع جميع الصفحات. |
| IgnoreBlank | `1` | لا تطبع الصفحات التي تكون الخلايا فيها فارغة. |
| IgnoreStyle | `2` | لا تطبع الصفحات التي تحتوي الخلايا فيها على الأنماط فقط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintingPageTypeDemo
    {
        public static void PrintingPageTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بعض البيانات في ورقة العمل
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            worksheet.Cells["A3"].PutValue("!");

            // إنشاء PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // عيّن PrintingPageType إلى IgnoreBlank
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;

            // احفظ المصنف كملف PDF باستخدام الخيارات المحددة
            workbook.Save("output_ignore_blank_page.pdf", pdfSaveOptions);

            // عيّن PrintingPageType إلى IgnoreStyle
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;

            // احفظ المصنف كملف PDF باستخدام الخيارات المحددة
            workbook.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);

            // عيّن PrintingPageType إلى Default
            pdfSaveOptions.PrintingPageType = PrintingPageType.Default;

            // احفظ المصنف كملف PDF باستخدام الخيارات المحددة
            workbook.Save("output_default_page.pdf", pdfSaveOptions);

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


