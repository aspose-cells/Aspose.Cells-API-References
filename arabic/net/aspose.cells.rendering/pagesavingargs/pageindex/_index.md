---
title: "PageSavingArgs.PageIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSavingArgs. فهرس الصفحة الحالي يبدأ من الصفر"
type: docs
url: /ar/net/aspose.cells.rendering/pagesavingargs/pageindex/
---
## PageSavingArgs.PageIndex property

فهرس الصفحة الحالي، يبدأ من الصفر.

```csharp
public int PageIndex { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSavingArgsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بعض البيانات إلى ورقة العمل
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // أنشئ خيارات حفظ PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // تعيين رد نداء حفظ الصفحة
            options.PageSavingCallback = new PageSavingCallback();

            // حفظ المصنف إلى PDF - سيؤدي ذلك إلى تشغيل رد النداء لكل صفحة
            workbook.Save("output.pdf", options);
        }
    }

    public class PageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            // عرض مثال لاستخدام خاصية PageIndex
            Console.WriteLine($"Starting to save page {args.PageIndex + 1}");
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // غير مستخدم في هذا المثال
        }
    }
}
```

### انظر أيضًا

* class [PageSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


