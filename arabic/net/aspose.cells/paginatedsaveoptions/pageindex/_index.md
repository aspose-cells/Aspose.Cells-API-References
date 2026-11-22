---
title: "PaginatedSaveOptions.PageIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaginatedSaveOptions. تحصل أو تعين الفهرس الصفري للصفحة الأولى التي سيتم حفظها"
type: docs
url: /ar/net/aspose.cells/paginatedsaveoptions/pageindex/
---
## PaginatedSaveOptions.PageIndex property

يحصل أو يضبط الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها.

```csharp
public int PageIndex { get; set; }
```

### ملاحظات

القيمة الافتراضية هي 0.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // أضف بيانات نموذجية عبر صفحات متعددة
            for (int i = 0; i < 100; i++)
            {
                sheet.Cells[i, 0].Value = "Data " + (i + 1);
            }

            // حدد خيارات حفظ PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // حدد لطباعة الصفحات 3-4 (فهرس صفري)
            options.PageIndex = 2;  // Third page (index 2)
            options.PageCount = 2; // Print 2 pages
            
            // احفظ ملف PDF مع الصفحات المحددة
            wb.Save("SelectedPages.pdf", options);
            
            Console.WriteLine("PDF with pages 3-4 created successfully.");
        }
    }
}
```

### انظر أيضًا

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


