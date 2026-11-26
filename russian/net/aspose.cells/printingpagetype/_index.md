---
title: "Перечисление PrintingPageType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.PrintingPageType. Указывает, какие страницы не будут печататься"
type: docs
url: /ru/net/aspose.cells/printingpagetype/
---
## PrintingPageType enumeration

Указывает, какие страницы не будут печататься.

```csharp
public enum PrintingPageType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Default | `0` | Печатает все страницы. |
| IgnoreBlank | `1` | Не печатать страницы, на которых ячейки пусты. |
| IgnoreStyle | `2` | Не печатать страницы, в которых ячейки содержат только стили. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintingPageTypeDemo
    {
        public static void PrintingPageTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните некоторые данные в листе
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            worksheet.Cells["A3"].PutValue("!");

            // Создать PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Установите PrintingPageType в значение IgnoreBlank
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;

            // Сохраните книгу в PDF с указанными параметрами
            workbook.Save("output_ignore_blank_page.pdf", pdfSaveOptions);

            // Установите PrintingPageType в значение IgnoreStyle
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;

            // Сохраните книгу в PDF с указанными параметрами
            workbook.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);

            // Установите PrintingPageType в значение Default
            pdfSaveOptions.PrintingPageType = PrintingPageType.Default;

            // Сохраните книгу в PDF с указанными параметрами
            workbook.Save("output_default_page.pdf", pdfSaveOptions);

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


