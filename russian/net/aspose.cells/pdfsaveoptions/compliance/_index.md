---
title: "PdfSaveOptions.Compliance"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSaveOptions. Получает или задает уровень соответствия стандартам PDF для выходных документов"
type: docs
url: /ru/net/aspose.cells/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

Получает или задаёт уровень соответствия стандартам PDF для выходных документов.

```csharp
public PdfCompliance Compliance { get; set; }
```

### Примечания

По умолчанию — Pdf17.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyComplianceDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с тестовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test PDF Compliance");

            // Установите параметры сохранения PDF с соответствием PDF/A-1b
            PdfSaveOptions options = new PdfSaveOptions
            {
                Compliance = PdfCompliance.PdfA1b
            };

            // Сохранить книгу в формате PDF с настройками соответствия
            workbook.Save("output.pdf", options);
            
            Console.WriteLine("PDF saved with PDF/A-1b compliance.");
        }
    }
}
```

### См. также

* enum [PdfCompliance](../../../aspose.cells.rendering/pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


