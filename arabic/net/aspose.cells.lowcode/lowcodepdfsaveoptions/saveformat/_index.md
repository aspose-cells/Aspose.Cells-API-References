---
title: "LowCodePdfSaveOptions.SaveFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodePdfSaveOptions. تنسيق الحفظ للمخرجات. لتحويل إلى pdf يمكن أن يكون فقط Pdf"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodepdfsaveoptions/saveformat/
---
## LowCodePdfSaveOptions.SaveFormat property

تنسيق الحفظ للإخراج. للتحويل إلى PDF، لا يمكن أن يكون إلا PDF.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodePdfSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Testing PDF SaveFormat Property");

            LowCodePdfSaveOptions pdfOptions = new LowCodePdfSaveOptions();

            Console.WriteLine("Current SaveFormat value: " + pdfOptions.SaveFormat);

            pdfOptions.SaveFormat = SaveFormat.Pdf;

            PdfSaveOptions options = pdfOptions.PdfOptions;
            options.Compliance = PdfCompliance.PdfA1a;

            workbook.Save("LowCodePdfSaveFormatDemo.pdf", options);
        }
    }
}
```

### انظر أيضًا

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodePdfSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


