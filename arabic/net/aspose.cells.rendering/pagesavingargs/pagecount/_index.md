---
title: "PageSavingArgs.PageCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSavingArgs. العدد الإجمالي للصفحات"
type: docs
url: /ar/net/aspose.cells.rendering/pagesavingargs/pagecount/
---
## PageSavingArgs.PageCount property

إجمالي عدد الصفحات.

```csharp
public int PageCount { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageSavingArgsPropertyPageCountDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد وإضافة بيانات اختبار
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة محتوى كثيف لإنشاء صفحات متعددة
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            // ضبط إعداد الصفحة للتحكم في التقسيم إلى صفحات
            worksheet.PageSetup.PrintArea = "A1:A50";
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            // إنشاء خيارات حفظ PDF مع رد نداء حفظ الصفحة
            PdfSaveOptions options = new PdfSaveOptions();
            options.PageSavingCallback = new PageSavingCallback();

            // حفظ إلى PDF لتفعيل تقسيم الصفحات
            workbook.Save("PageSavingDemo.pdf", options);
        }

        private class PageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                // الوصول إلى PageCount من معلمات الحدث
                Console.WriteLine($"Saving page {args.PageIndex + 1} of {args.PageCount}");
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // لا حاجة إلى تنفيذ
            }
        }
    }
}
```

### انظر أيضًا

* class [PageSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


