---
title: "PdfSaveOptions.FontEncoding"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSaveOptions. Получает или задает встроенную кодировку шрифтов в PDF"
type: docs
url: /ru/net/aspose.cells/pdfsaveoptions/fontencoding/
---
## PdfSaveOptions.FontEncoding property

Получает или задаёт кодировку встроенных шрифтов в PDF.

```csharp
public PdfFontEncoding FontEncoding { get; set; }
```

### Примечания

Значение по умолчанию — Identity

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyFontEncodingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Font Encoding Test");
            worksheet.Cells["A2"].PutValue("This demonstrates PdfFontEncoding usage");

            // Настройте параметры сохранения PDF с помощью FontEncoding
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.FontEncoding = PdfFontEncoding.Identity;
            pdfSaveOptions.DefaultFont = "Arial";

            // Сохраните книгу в PDF
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### См. также

* enum [PdfFontEncoding](../../../aspose.cells.rendering/pdffontencoding/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


