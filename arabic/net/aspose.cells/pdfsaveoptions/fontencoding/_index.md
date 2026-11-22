---
title: "PdfSaveOptions.FontEncoding"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSaveOptions. تحصل أو تعيين ترميز الخط المضمن في pdf"
type: docs
url: /ar/net/aspose.cells/pdfsaveoptions/fontencoding/
---
## PdfSaveOptions.FontEncoding property

يحصل على أو يضبط ترميز الخط المضمن في PDF.

```csharp
public PdfFontEncoding FontEncoding { get; set; }
```

### ملاحظات

القيمة الافتراضية هي Identity

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyFontEncodingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Font Encoding Test");
            worksheet.Cells["A2"].PutValue("This demonstrates PdfFontEncoding usage");

            // تكوين خيارات حفظ PDF مع FontEncoding
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.FontEncoding = PdfFontEncoding.Identity;
            pdfSaveOptions.DefaultFont = "Arial";

            // احفظ المصنف كملف PDF
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### انظر أيضًا

* enum [PdfFontEncoding](../../../aspose.cells.rendering/pdffontencoding/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


