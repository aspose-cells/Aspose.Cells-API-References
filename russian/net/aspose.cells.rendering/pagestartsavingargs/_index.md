---
title: "Класс PageStartSavingArgs"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Rendering.PageStartSavingArgs. Информация о начале процесса сохранения страницы"
type: docs
url: /ru/net/aspose.cells.rendering/pagestartsavingargs/
---
## PageStartSavingArgs class

Информация о начале процесса сохранения страницы.

```csharp
public class PageStartSavingArgs : PageSavingArgs
```

## Свойства

| Имя | Описание |
| --- | --- |
| [IsToOutput](../../aspose.cells.rendering/pagestartsavingargs/istooutput/) { get; set; } | Получает или задаёт значение, указывающее, должна ли страница выводиться. Значение по умолчанию — true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Общее количество страниц.(Унаследовано от [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Текущий индекс страницы, начиная с нуля.(Унаследовано от [`PageSavingArgs`](../pagesavingargs/).) |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassPageStartSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue("Hello World");
            
            PdfSaveOptions options = new PdfSaveOptions();
            options.PageSavingCallback = new CustomPageSavingCallback();
            
            workbook.Save("output.pdf", options);
        }
    }
    
    public class CustomPageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex}");
        }
        
        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Необязательная реализация
        }
    }
}
```

### См. также

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


