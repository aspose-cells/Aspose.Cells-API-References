---
title: "PaginatedSaveOptions.GridlineType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaginatedSaveOptions. تحصل أو تعيين نوع خطوط الشبكة"
type: docs
url: /ar/net/aspose.cells/paginatedsaveoptions/gridlinetype/
---
## PaginatedSaveOptions.GridlineType property

يحصل أو يضبط نوع خطوط الشبكة.

```csharp
public GridlineType GridlineType { get; set; }
```

### ملاحظات

القيمة الافتراضية هي النوع المنقط.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyGridlineTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات عينة وفعل خطوط الشبكة
            worksheet.Cells["A1"].PutValue("GridlineType Demo");
            worksheet.Cells["B2"].PutValue(1);
            worksheet.Cells["C3"].PutValue(2);
            worksheet.Cells["D4"].PutValue(3);
            worksheet.IsGridlinesVisible = true;

            // أنشئ خيارات حفظ PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // عرض خاصية GridlineType
            pdfSaveOptions.GridlineType = GridlineType.Dotted;

            // احفظ دفتر العمل مع خطوط الشبكة
            workbook.Save("GridlineTypeDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### انظر أيضًا

* enum [GridlineType](../../gridlinetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


