---
title: "PaginatedSaveOptions.PageIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Получает или задает индекс первой страницы для сохранения, нумерация начинается с нуля"
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/pageindex/
---
## PaginatedSaveOptions.PageIndex property

Получает или задает нулевой индекс первой страницы для сохранения.

```csharp
public int PageIndex { get; set; }
```

### Примечания

По умолчанию 0.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Добавьте примерные данные на несколько страниц
            for (int i = 0; i < 100; i++)
            {
                sheet.Cells[i, 0].Value = "Data " + (i + 1);
            }

            // Установите параметры сохранения PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Установите печать страниц 3‑4 (нумерация с нуля)
            options.PageIndex = 2;  // Third page (index 2)
            options.PageCount = 2; // Print 2 pages
            
            // Сохраните PDF с выбранными страницами
            wb.Save("SelectedPages.pdf", options);
            
            Console.WriteLine("PDF with pages 3-4 created successfully.");
        }
    }
}
```

### См. также

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


