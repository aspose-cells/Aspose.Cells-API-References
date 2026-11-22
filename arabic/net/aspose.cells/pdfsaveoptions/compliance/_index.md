---
title: "PdfSaveOptions.Compliance"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSaveOptions. تحصل أو تعيّن مستوى الامتثال لمعايير PDF للمستندات الناتجة"
type: docs
url: /ar/net/aspose.cells/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

يحصل على أو يضبط مستوى التوافق مع معايير PDF للمستندات الناتجة.

```csharp
public PdfCompliance Compliance { get; set; }
```

### ملاحظات

القيمة الافتراضية هي Pdf17.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyComplianceDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل تجريبي مع بيانات اختبار
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test PDF Compliance");

            // عيّن خيارات حفظ PDF مع الامتثال PDF/A-1b
            PdfSaveOptions options = new PdfSaveOptions
            {
                Compliance = PdfCompliance.PdfA1b
            };

            // احفظ المصنف كملف PDF مع إعدادات الامتثال
            workbook.Save("output.pdf", options);
            
            Console.WriteLine("PDF saved with PDF/A-1b compliance.");
        }
    }
}
```

### انظر أيضًا

* enum [PdfCompliance](../../../aspose.cells.rendering/pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


