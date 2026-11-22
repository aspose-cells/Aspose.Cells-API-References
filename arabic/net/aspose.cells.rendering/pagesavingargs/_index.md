---
title: "الفئة PageSavingArgs"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Rendering.PageSavingArgs. معلومات حول عملية حفظ الصفحة"
type: docs
url: /ar/net/aspose.cells.rendering/pagesavingargs/
---
## PageSavingArgs class

معلومات حول عملية حفظ الصفحة.

```csharp
public class PageSavingArgs
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | إجمالي عدد الصفحات. |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | فهرس الصفحة الحالي، يبدأ من الصفر. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassPageSavingArgsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد ببيانات موسعة لعدة صفحات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء ورقة العمل لتوليد عدة صفحات عند العرض
            for (int row = 0; row < 150; row++)
            {
                worksheet.Cells[row, 0].Value = $"Row {row + 1} data";
            }

            // تكوين خيارات حفظ PDF مع رد نداء حفظ الصفحة
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.PageSavingCallback = new PageSavingCallback();

            // احفظ دفتر العمل بتنسيق PDF مع ترقيم الصفحات
            workbook.Save("RenderingPageSavingDemo.pdf", pdfSaveOptions);
        }

        private class PageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                Console.WriteLine($"Saving page {args.PageIndex + 1} of {args.PageCount}");
                
                if (args.PageIndex == 0)
                {
                    Console.WriteLine("Processing cover page...");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // اختياري: أضف أي معالجة لنهاية الصفحة هنا
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


