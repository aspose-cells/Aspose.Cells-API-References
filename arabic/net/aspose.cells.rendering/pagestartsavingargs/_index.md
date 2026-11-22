---
title: "فئة PageStartSavingArgs"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Rendering.PageStartSavingArgs. معلومات لبدء عملية حفظ الصفحة"
type: docs
url: /ar/net/aspose.cells.rendering/pagestartsavingargs/
---
## PageStartSavingArgs class

معلومات حول بدء عملية حفظ الصفحة.

```csharp
public class PageStartSavingArgs : PageSavingArgs
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [IsToOutput](../../aspose.cells.rendering/pagestartsavingargs/istooutput/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إخراج الصفحة. القيمة الافتراضية هي true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | إجمالي عدد الصفحات.(موروث من [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | فهرس الصفحة الحالية، يبدأ من الصفر.(موروث من [`PageSavingArgs`](../pagesavingargs/).) |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassPageStartSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("Hello World");
            
            PdfSaveOptions options = new PdfSaveOptions();
            options.PageSavingCallback = new CustomPageSavingCallback();
            
            workbook.Save("output.pdf", options);
        }
    }
    
    public class CustomPageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex}");
        }
        
        public void PageEndSaving(PageEndSavingArgs args)
        {
            // تنفيذ اختياري
        }
    }
}
```

### انظر أيضًا

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


