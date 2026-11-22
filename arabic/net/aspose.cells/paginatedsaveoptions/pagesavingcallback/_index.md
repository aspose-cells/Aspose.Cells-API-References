---
title: "PaginatedSaveOptions.PageSavingCallback"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaginatedSaveOptions. التحكم/الإشارة إلى تقدم عملية حفظ الصفحات"
type: docs
url: /ar/net/aspose.cells/paginatedsaveoptions/pagesavingcallback/
---
## PaginatedSaveOptions.PageSavingCallback property

التحكم/الإشارة إلى تقدم عملية حفظ الصفحة.

```csharp
public IPageSavingCallback PageSavingCallback { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageSavingCallbackDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            worksheet.Cells["A2"].PutValue("This demonstrates PageSavingCallback");

            // أنشئ خيارات الحفظ مع رد نداء حفظ الصفحات
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new CustomPageSavingCallback();

            // احفظ باستخدام رد النداء
            workbook.Save("PageSavingCallbackDemo.pdf", saveOptions);
        }
    }

    public class CustomPageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex + 1}");
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex + 1}");
            if (args.HasMorePages)
            {
                Console.WriteLine("More pages to follow...");
            }
        }
    }
}
```

### انظر أيضًا

* interface [IPageSavingCallback](../../../aspose.cells.rendering/ipagesavingcallback/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


