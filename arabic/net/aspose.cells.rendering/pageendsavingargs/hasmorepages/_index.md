---
title: "PageEndSavingArgs.HasMorePages"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageEndSavingArgs. تحصل أو تعيين قيمة تشير إلى ما إذا كان هناك صفحات إضافية ليتم إخراجها. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells.rendering/pageendsavingargs/hasmorepages/
---
## PageEndSavingArgs.HasMorePages property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان هناك المزيد من الصفحات ليتم إخراجها. القيمة الافتراضية هي true.

```csharp
public bool HasMorePages { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageEndSavingArgsPropertyHasMorePagesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل يحتوي على بيانات تمتد عبر عدة صفحات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[i, 0].Value = $"Row {i + 1}";
            }

            // إنشاء خيارات حفظ PDF مع معالجة صفحات مخصصة
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new PageControlCallback();

            // حفظ دفتر العمل مع تحديد عدد الصفحات
            workbook.Save("PropertyHasMorePagesDemo.pdf", saveOptions);
        }
    }

    internal class PageControlCallback : IPageSavingCallback
    {
        private int pageCount = 0;

        public void PageStartSaving(PageStartSavingArgs args)
        {
            // غير مستخدم في هذا العرض
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // قراءة قيمة الخاصية الحالية
            Console.WriteLine($"Page {pageCount} - Initial HasMorePages: {args.HasMorePages}");

            // تعديل الخاصية بعد الصفحة الأولى
            if (pageCount == 0)
            {
                args.HasMorePages = false;
                Console.WriteLine($"Page {pageCount} - Updated HasMorePages: {args.HasMorePages}");
            }

            pageCount++;
        }
    }
}
```

### انظر أيضًا

* class [PageEndSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


