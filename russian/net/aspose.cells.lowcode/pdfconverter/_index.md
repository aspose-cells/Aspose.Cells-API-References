---
title: "Класс PdfConverter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.LowCode.PdfConverter. Конвертер для преобразования файла шаблона в PDF"
type: docs
url: /ru/net/aspose.cells.lowcode/pdfconverter/
---
## PdfConverter class

Конвертер для преобразования шаблонного файла в PDF.

```csharp
public class PdfConverter
```

## Методы

| Имя | Описание |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Преобразует файл шаблона в PDF |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process_1)(string, string) | Преобразует указанный файл шаблона в PDF. |

### Примеры

```csharp
using System;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassPdfConverterDemo
    {
        public static void Run()
        {
            // Инициализировать PdfConverter с путями к шаблону и выходному файлу
            PdfConverter.Process("template.xlsx", "res.pdf");
            
            Console.WriteLine("PDF conversion completed successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


