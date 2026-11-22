---
title: "PaginatedSaveOptions.PageCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaginatedSaveOptions. تحصل أو تعين عدد الصفحات التي سيتم حفظها"
type: docs
url: /ar/net/aspose.cells/paginatedsaveoptions/pagecount/
---
## PaginatedSaveOptions.PageCount property

يحصل أو يضبط عدد الصفحات التي سيتم حفظها.

```csharp
public int PageCount { get; set; }
```

### ملاحظات

القيمة الافتراضية هي System.Int32.MaxValue مما يعني أنه سيتم تصيير جميع الصفحات..

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageCountDemo
    {
        public static void Run()
        {
            // افتح ملف Excel
            Workbook wb = new Workbook("Book1.xlsx");
            
            // تهيئة خيارات حفظ PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // عيّن للطباعة صفحتين فقط بدءًا من الصفحة 4 (الفهرس صفر-مبني 3)
            options.PageIndex = 3;
            options.PageCount = 2;
            
            // احفظ ملف PDF
            wb.Save("output.pdf", options);
            
            Console.WriteLine("PDF saved with selected pages.");
        }
    }
}
```

### انظر أيضًا

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


