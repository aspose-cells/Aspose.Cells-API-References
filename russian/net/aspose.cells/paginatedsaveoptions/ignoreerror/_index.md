---
title: "PaginatedSaveOptions.IgnoreError"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Указывает, нужно ли скрывать ошибку при рендеринге. Ошибка может быть ошибкой при рендеринге фигур, изображений, диаграмм и т.д."
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/ignoreerror/
---
## PaginatedSaveOptions.IgnoreError property

Указывает, нужно ли скрывать ошибку во время рендеринга. Ошибка может быть связана с формой, изображением, рендерингом диаграммы и т.д.

```csharp
public bool IgnoreError { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyIgnoreErrorDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые примерные данные с потенциальными ошибками форматирования
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);
            
            // Создайте параметры сохранения PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Установите IgnoreError в true, чтобы пропустить любые ошибки конвертации
            options.IgnoreError = true;
            
            // Сохранить книгу в формате PDF
            workbook.Save("PaginatedSaveWithIgnoreError.pdf", options);
            
            Console.WriteLine("PDF saved with IgnoreError enabled.");
        }
    }
}
```

### См. также

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


