---
title: "PaginatedSaveOptions.CheckWorkbookDefaultFont"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Когда символы в Excel являются Unicode и не заданы правильным шрифтом в стиле ячейки, они могут отображаться как блоки в pdfimage. Установите значение true, чтобы попытаться использовать шрифт по умолчанию книги для отображения этих символов."
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/
---
## PaginatedSaveOptions.CheckWorkbookDefaultFont property

Когда символы в Excel являются Unicode и для них не установлен корректный шрифт в стиле ячейки, они могут отображаться как блоки в PDF, изображении. Установите значение true, чтобы попытаться сначала использовать шрифт по умолчанию книги для отображения этих символов.

```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```

### Примечания

По умолчанию true.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyCheckWorkbookDefaultFontDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Test Content");
            
            // Настройте параметры сохранения PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.CheckWorkbookDefaultFont = false;
            
            // Сохранить в PDF
            workbook.Save("output.pdf", saveOptions);
            
            Console.WriteLine("PDF saved with CheckWorkbookDefaultFont set to false");
        }
    }
}
```

### См. также

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


