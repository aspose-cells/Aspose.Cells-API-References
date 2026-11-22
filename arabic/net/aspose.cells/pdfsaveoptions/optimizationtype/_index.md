---
title: "PdfSaveOptions.OptimizationType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSaveOptions. تحصل وتعيين نوع تحسين pdf"
type: docs
url: /ar/net/aspose.cells/pdfsaveoptions/optimizationtype/
---
## PdfSaveOptions.OptimizationType property

يحصل على ويضبط نوع تحسين PDF.

```csharp
public PdfOptimizationType OptimizationType { get; set; }
```

### ملاحظات

القيمة الافتراضية هي Standard

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyOptimizationTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Optimization Example");

            // أنشئ خيارات حفظ PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // عرض خاصية OptimizationType
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;

            // حفظ المصنف مع إعدادات التحسين
            workbook.Save("OptimizedPdf.pdf", pdfSaveOptions);
        }
    }
}
```

### انظر أيضًا

* enum [PdfOptimizationType](../../../aspose.cells.rendering/pdfoptimizationtype/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


