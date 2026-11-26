---
title: "PaginatedSaveOptions.DefaultFont"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Когда символы в Excel являются Unicode и в стиле ячейки не установлен корректный шрифт, они могут отображаться как блоки в pdfimage. Установите DefaultFont, например MingLiu или MS Gothic, чтобы отобразить эти символы. Если это свойство не задано, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих Unicode‑символов."
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/defaultfont/
---
## PaginatedSaveOptions.DefaultFont property

Когда символы в Excel являются Unicode и для них не установлен корректный шрифт в стиле ячейки, они могут отображаться как блоки в PDF, изображении. Установите свойство DefaultFont, например MingLiu или MS Gothic, чтобы отобразить эти символы. Если это свойство не задано, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих Unicode‑символов.

```csharp
public string DefaultFont { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyDefaultFontDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("This text will use the default font");
            worksheet.Cells["A2"].PutValue("如果默认字体支持中文，这将显示正确");

            // Настройте параметры сохранения PDF с шрифтом по умолчанию
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.DefaultFont = "宋体";
            pdfSaveOptions.CheckWorkbookDefaultFont = true;

            // Сохранить в PDF
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### См. также

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


