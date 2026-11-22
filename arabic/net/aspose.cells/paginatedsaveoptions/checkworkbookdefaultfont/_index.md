---
title: "PaginatedSaveOptions.CheckWorkbookDefaultFont"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaginatedSaveOptions. عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية قد تظهر ككتل في pdfimage. عيّن هذا إلى true لمحاولة استخدام الخط الافتراضي للدفتر لإظهار هذه الأحرف أولاً"
type: docs
url: /ar/net/aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/
---
## PaginatedSaveOptions.CheckWorkbookDefaultFont property

عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdf أو صورة. اضبط هذا على true لمحاولة استخدام الخط الافتراضي لدفتر العمل لعرض هذه الأحرف أولاً.

```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```

### ملاحظات

القيمة الافتراضية هي true.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyCheckWorkbookDefaultFontDemo
    {
        public static void Run()
        {
            // إنشاء مصنف تجريبي
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Test Content");
            
            // تكوين خيارات حفظ PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.CheckWorkbookDefaultFont = false;
            
            // احفظ إلى PDF
            workbook.Save("output.pdf", saveOptions);
            
            Console.WriteLine("PDF saved with CheckWorkbookDefaultFont set to false");
        }
    }
}
```

### انظر أيضًا

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


