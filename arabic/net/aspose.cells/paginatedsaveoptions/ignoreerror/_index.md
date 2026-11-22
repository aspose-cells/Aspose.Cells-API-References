---
title: "PaginatedSaveOptions.IgnoreError"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaginatedSaveOptions. تشير إلى ما إذا كنت بحاجة إلى إخفاء الخطأ أثناء العرض. قد يكون الخطأ في شكل أو صورة أو رسم بياني أو غير ذلك أثناء العرض"
type: docs
url: /ar/net/aspose.cells/paginatedsaveoptions/ignoreerror/
---
## PaginatedSaveOptions.IgnoreError property

يشير إلى ما إذا كنت بحاجة إلى إخفاء الخطأ أثناء التصيير. قد يكون الخطأ في الشكل أو الصورة أو تصيير المخطط، إلخ.

```csharp
public bool IgnoreError { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyIgnoreErrorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات النموذجية مع أخطاء تنسيق محتملة
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);
            
            // أنشئ خيارات حفظ PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // عيّن IgnoreError إلى true لتجاوز أي أخطاء تحويل
            options.IgnoreError = true;
            
            // احفظ المصنف كملف PDF
            workbook.Save("PaginatedSaveWithIgnoreError.pdf", options);
            
            Console.WriteLine("PDF saved with IgnoreError enabled.");
        }
    }
}
```

### انظر أيضًا

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


