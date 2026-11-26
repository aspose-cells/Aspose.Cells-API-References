---
title: "LowCodePdfSaveOptions.SaveFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodePdfSaveOptions. Формат сохранения для вывода. При конвертации в PDF может быть только Pdf"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodepdfsaveoptions/saveformat/
---
## LowCodePdfSaveOptions.SaveFormat property

Формат сохранения для вывода. При конвертации в PDF он может быть только PDF.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### Примеры

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

### См. также

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodePdfSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


