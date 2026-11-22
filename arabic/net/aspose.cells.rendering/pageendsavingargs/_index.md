---
title: "الفئة PageEndSavingArgs"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Rendering.PageEndSavingArgs. معلومات حول عملية إنهاء حفظ الصفحة"
type: docs
url: /ar/net/aspose.cells.rendering/pageendsavingargs/
---
## PageEndSavingArgs class

معلومات الصفحة تنهي عملية الحفظ.

```csharp
public class PageEndSavingArgs : PageSavingArgs
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [HasMorePages](../../aspose.cells.rendering/pageendsavingargs/hasmorepages/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان هناك المزيد من الصفحات ليتم إخراجها. القيمة الافتراضية هي true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | إجمالي عدد الصفحات.(موروث من [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | فهرس الصفحة الحالية، يبدأ من الصفر.(موروث من [`PageSavingArgs`](../pagesavingargs/).) |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassPageEndSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // إنشاء كائن من PdfSaveOptions
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // تعيين رد النداء PageEndSaving
            saveOptions.PageSavingCallback = new PageEndSavingArgsTest();

            // احفظ المصنف باستخدام رد النداء
            workbook.Save("output.pdf", saveOptions);
        }
    }

    public class PageEndSavingArgsTest : IPageSavingCallback
    {
        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex}");
        }

        public void PageStartSaving(PageStartSavingArgs args)
        {
            // لا يلزم تنفيذ لهذا العرض التوضيحي
        }
    }
}
```

### انظر أيضًا

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


