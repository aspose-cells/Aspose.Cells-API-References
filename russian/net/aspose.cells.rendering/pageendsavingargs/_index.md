---
title: "Класс PageEndSavingArgs"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Rendering.PageEndSavingArgs. Информация о завершении процесса сохранения страницы"
type: docs
url: /ru/net/aspose.cells.rendering/pageendsavingargs/
---
## PageEndSavingArgs class

Информация о странице завершает процесс сохранения.

```csharp
public class PageEndSavingArgs : PageSavingArgs
```

## Свойства

| Имя | Описание |
| --- | --- |
| [HasMorePages](../../aspose.cells.rendering/pageendsavingargs/hasmorepages/) { get; set; } | Получает или задает значение, указывающее, есть ли ещё страницы для вывода. Значение по умолчанию — true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Общее количество страниц.(Унаследовано от [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Текущий индекс страницы, начиная с нуля.(Унаследовано от [`PageSavingArgs`](../pagesavingargs/).) |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassPageEndSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Создайте экземпляр PdfSaveOptions
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Установите обратный вызов PageEndSaving
            saveOptions.PageSavingCallback = new PageEndSavingArgsTest();

            // Сохраните книгу с обратным вызовом
            workbook.Save("output.pdf", saveOptions);
        }
    }

    public class PageEndSavingArgsTest : IPageSavingCallback
    {
        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex}");
        }

        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Реализация не требуется для этой демонстрации
        }
    }
}
```

### См. также

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


