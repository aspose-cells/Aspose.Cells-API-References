---
title: "PdfSaveOptions.DisplayDocTitle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSaveOptions. تشير إلى ما إذا كان شريط عنوان النوافذ يجب أن يعرض عنوان المستند"
type: docs
url: /ar/net/aspose.cells/pdfsaveoptions/displaydoctitle/
---
## PdfSaveOptions.DisplayDocTitle property

يشير إلى ما إذا كان شريط عنوان النافذة يجب أن يعرض عنوان المستند.

```csharp
public bool DisplayDocTitle { get; set; }
```

### ملاحظات

إذا كانت false، يجب أن يعرض شريط العنوان بدلاً من ذلك اسم ملف PDF. القيمة الافتراضية هي false.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyDisplayDocTitleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF DisplayDocTitle Example");

            // أنشئ خيارات حفظ PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // عيّن خاصية DisplayDocTitle إلى true
            pdfSaveOptions.DisplayDocTitle = true;

            // احفظ المصنف كملف PDF
            workbook.Save("PdfDisplayDocTitleDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### انظر أيضًا

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


