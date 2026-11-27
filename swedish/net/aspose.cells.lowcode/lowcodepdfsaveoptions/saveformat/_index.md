---
title: "LowCodePdfSaveOptions.SaveFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodePdfSaveOptions egenskap. Sparaformatet för utdata. Vid konvertering till pdf kan det endast vara Pdf"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodepdfsaveoptions/saveformat/
---
## LowCodePdfSaveOptions.SaveFormat property

Sparaformatet för utdata. För konvertering till PDF kan det endast vara PDF.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### Exempel

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

### Se även

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodePdfSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


