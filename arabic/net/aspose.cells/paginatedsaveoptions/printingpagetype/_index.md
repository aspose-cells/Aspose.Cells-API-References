---
title: "PaginatedSaveOptions.PrintingPageType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaginatedSaveOptions. تشير إلى الصفحات التي لن يتم طباعتها"
type: docs
url: /ar/net/aspose.cells/paginatedsaveoptions/printingpagetype/
---
## PaginatedSaveOptions.PrintingPageType property

يشير إلى الصفحات التي لن تُطبع.

```csharp
public PrintingPageType PrintingPageType { get; set; }
```

### ملاحظات

إذا كان المحتوى في الورقة متفرقًا، قد تكون هناك بعض الصفحات فارغة تمامًا في ملف PDF الناتج. إذا كنت لا تريد هذه الصفحات الفارغة، يمكنك استخدام هذا الخيار لتخطيها.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPrintingPageTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // أضف بعض البيانات التجريبية
            ws.Cells["A1"].PutValue("Sample Data");
            ws.Cells["A2"].PutValue(123);
            ws.Cells["A3"].PutValue(456);
            
            // إنشاء ورقة عمل فارغة
            Worksheet blankWs = wb.Worksheets.Add("BlankSheet");
            
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // احفظ متجاهلًا الصفحات الفارغة
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            wb.Save("output_ignore_blank_page.pdf", pdfSaveOptions);
            
            // احفظ متجاهلًا الصفحات الفارغة والصفحات التي تحتوي على نمط فقط
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;
            wb.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
        }
    }
}
```

### انظر أيضًا

* enum [PrintingPageType](../../printingpagetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


