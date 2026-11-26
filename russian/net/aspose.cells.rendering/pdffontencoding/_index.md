---
title: "Перечисление PdfFontEncoding"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Rendering.PdfFontEncoding. Представляет кодировку встроенных шрифтов PDF"
type: docs
url: /ru/net/aspose.cells.rendering/pdffontencoding/
---
## PdfFontEncoding enumeration

Представляет кодировку встроенного шрифта PDF.

```csharp
public enum PdfFontEncoding
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Identity | `0` | Представляет использование кодировки Identity-H для всех встроенных шрифтов в PDF. |
| AnsiPrefer | `1` | Представляет предпочтение использования WinAnsiEncoding для TrueType‑шрифтов с символами 32‑127; в остальных случаях будет использоваться кодировка Identity-H для встроенных шрифтов в PDF. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfFontEncodingDemo
    {
        public static void PdfFontEncodingExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello, Aspose!");

            // Создайте PdfSaveOptions и установите свойство FontEncoding
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.FontEncoding = PdfFontEncoding.AnsiPrefer;

            // Сохраните рабочую книгу в виде PDF-файла
            workbook.Save("PdfFontEncodingExample.pdf", pdfSaveOptions);

            Console.WriteLine("PDF file created successfully with specified font encoding.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


