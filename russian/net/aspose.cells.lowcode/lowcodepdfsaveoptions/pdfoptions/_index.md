---
title: "LowCodePdfSaveOptions.PdfOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodePdfSaveOptions. Параметры для сохранения PDF‑файла"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodepdfsaveoptions/pdfoptions/
---
## LowCodePdfSaveOptions.PdfOptions property

Параметры сохранения PDF-файла.

```csharp
public PdfSaveOptions PdfOptions { get; set; }
```

### Примеры

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
            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF Options Demo");

            // Создать параметры сохранения PDF с пользовательскими настройками
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions
            {
                Compliance = PdfCompliance.PdfA1b,
                OnePagePerSheet = true
            };

            // Создать параметры сохранения PDF в low code и назначить параметры PDF
            LowCodePdfSaveOptions lowCodePdfSaveOptions = new LowCodePdfSaveOptions
            {
                OutputFile = "output.pdf",
                PdfOptions = pdfSaveOptions
            };

            // Сохранить, используя параметры low code
            workbook.Save(lowCodePdfSaveOptions.OutputFile, lowCodePdfSaveOptions.PdfOptions);

            Console.WriteLine("PDF saved with custom options.");
        }
    }
}
```

### См. также

* class [PdfSaveOptions](../../../aspose.cells/pdfsaveoptions/)
* class [LowCodePdfSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


