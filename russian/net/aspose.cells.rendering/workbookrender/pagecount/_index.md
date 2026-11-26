---
title: "WorkbookRender.PageCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookRender. Получает общее количество страниц книги"
type: docs
url: /ru/net/aspose.cells.rendering/workbookrender/pagecount/
---
## WorkbookRender.PageCount property

Получает общее количество страниц книги.

```csharp
public int PageCount { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderPropertyPageCountDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            
            // Добавить второй лист
            workbook.Worksheets.Add();
            worksheet = workbook.Worksheets[1];
            worksheet.Cells["A1"].PutValue("Page 2 Content");

            // Создать параметры рендеринга и рендерер книги
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true
            };
            
            WorkbookRender renderer = new WorkbookRender(workbook, options);

            // Продемонстрировать использование PageCount
            Console.WriteLine($"Total pages to render: {renderer.PageCount}");
            
            // Отрендерить каждую страницу в изображение
            for (int i = 0; i < renderer.PageCount; i++)
            {
                string outputPath = $"Page_{i}.png";
                renderer.ToImage(i, outputPath);
                Console.WriteLine($"Rendered page {i+1} to {outputPath}");
            }
        }
    }
}
```

### См. также

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


