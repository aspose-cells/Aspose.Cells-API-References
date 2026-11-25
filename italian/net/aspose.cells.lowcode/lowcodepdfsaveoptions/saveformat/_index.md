---
title: "LowCodePdfSaveOptions.SaveFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodePdfSaveOptions. Il formato di salvataggio per l'output. Per la conversione in pdf può essere solo Pdf"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodepdfsaveoptions/saveformat/
---
## LowCodePdfSaveOptions.SaveFormat property

Il formato di salvataggio per l'output. Per la conversione in PDF, può essere solo PDF.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### Esempi

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

### Vedi anche

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodePdfSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


