---
title: "PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Указывает, следует ли выводить пустую страницу, когда нечего печатать"
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/
---
## PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint property

Указывает, следует ли выводить пустую страницу, когда нечего печатать.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### Примечания

По умолчанию true.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте лист и скройте его (симулируя отсутствие содержимого для печати)
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.IsVisible = false;

            // Установите параметры сохранения PDF с OutputBlankPageWhenNothingToPrint = false
            PdfSaveOptions options = new PdfSaveOptions
            {
                OutputBlankPageWhenNothingToPrint = false
            };

            // Сохраните в PDF — пустая страница не должна быть создана
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputNoBlankPage.pdf");
            workbook.Save(outputPath, options);

            // Измените параметр на true
            options.OutputBlankPageWhenNothingToPrint = true;

            // Сохранить снова — должна быть сгенерирована пустая страница
            outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputWithBlankPage.pdf");
            workbook.Save(outputPath, options);
        }
    }
}
```

### См. также

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


