---
title: "LowCodePdfSaveOptions.SaveFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodePdfSaveOptions. El formato de guardado para la salida. Para convertir a pdf solo puede ser Pdf"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodepdfsaveoptions/saveformat/
---
## LowCodePdfSaveOptions.SaveFormat property

El formato de guardado para la salida. Para convertir a PDF, solo puede ser PDF.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### Ejemplos

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

### Ver también

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodePdfSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


