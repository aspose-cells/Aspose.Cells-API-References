---
title: "PdfSaveOptions.PdfSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор PdfSaveOptions. Создаёт параметры для сохранения PDF‑файла"
type: docs
url: /ru/net/aspose.cells/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

Создаёт параметры для сохранения PDF‑файла.

```csharp
public PdfSaveOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Продемонстрировать конструктор PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Compliance = PdfCompliance.PdfA1b;
            
            // Сохранить книгу с параметрами PDF
            workbook.Save("output.pdf", pdfSaveOptions);
            
            Console.WriteLine("PDF saved successfully with PdfA1b compliance.");
        }
    }
}
```

### См. также

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


