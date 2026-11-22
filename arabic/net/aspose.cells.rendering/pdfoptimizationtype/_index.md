---
title: "تعداد PdfOptimizationType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Rendering.PdfOptimizationType. يحدد نوعًا من التحسين"
type: docs
url: /ar/net/aspose.cells.rendering/pdfoptimizationtype/
---
## PdfOptimizationType enumeration

يحدد نوعًا من التحسين.

```csharp
public enum PdfOptimizationType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Standard | `0` | جودة طباعة عالية |
| MinimumSize | `1` | حجم الملف أهم من جودة الطباعة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfOptimizationTypeDemo
    {
        public static void PdfOptimizationTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // إنشاء PdfSaveOptions وتعيين نوع التحسين
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;

            // حفظ دفتر العمل كملف PDF مع نوع التحسين المحدد
            workbook.Save("OptimizedOutput.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with optimization type: MinimumSize");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


