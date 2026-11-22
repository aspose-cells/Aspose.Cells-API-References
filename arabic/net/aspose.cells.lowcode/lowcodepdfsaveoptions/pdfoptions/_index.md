---
title: "LowCodePdfSaveOptions.PdfOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodePdfSaveOptions. الخيارات لحفظ ملف Pdf"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodepdfsaveoptions/pdfoptions/
---
## LowCodePdfSaveOptions.PdfOptions property

الخيارات لحفظ ملف PDF.

```csharp
public PdfSaveOptions PdfOptions { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodePdfSaveOptionsPropertyPdfOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF Options Demo");

            // إنشاء خيارات حفظ PDF بإعدادات مخصصة
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions
            {
                Compliance = PdfCompliance.PdfA1b,
                OnePagePerSheet = true
            };

            // إنشاء خيارات حفظ PDF منخفض الشيفرة وتعيين خيارات PDF
            LowCodePdfSaveOptions lowCodePdfSaveOptions = new LowCodePdfSaveOptions
            {
                OutputFile = "output.pdf",
                PdfOptions = pdfSaveOptions
            };

            // حفظ باستخدام خيارات منخفضة الشيفرة
            workbook.Save(lowCodePdfSaveOptions.OutputFile, lowCodePdfSaveOptions.PdfOptions);

            Console.WriteLine("PDF saved with custom options.");
        }
    }
}
```

### انظر أيضًا

* class [PdfSaveOptions](../../../aspose.cells/pdfsaveoptions/)
* class [LowCodePdfSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


