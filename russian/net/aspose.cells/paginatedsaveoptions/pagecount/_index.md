---
title: "PaginatedSaveOptions.PageCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Получает или задает количество страниц для сохранения"
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/pagecount/
---
## PaginatedSaveOptions.PageCount property

Получает или задает количество страниц для сохранения.

```csharp
public int PageCount { get; set; }
```

### Примечания

По умолчанию System.Int32.MaxValue, что означает, что будут отрисованы все страницы.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageCountDemo
    {
        public static void Run()
        {
            // Откройте файл Excel
            Workbook wb = new Workbook("Book1.xlsx");
            
            // Инициализируйте параметры сохранения PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Установите печать только 2 страниц, начиная с страницы 4 (индекс 3, нумерация с нуля)
            options.PageIndex = 3;
            options.PageCount = 2;
            
            // Сохраните PDF‑файл
            wb.Save("output.pdf", options);
            
            Console.WriteLine("PDF saved with selected pages.");
        }
    }
}
```

### См. также

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


