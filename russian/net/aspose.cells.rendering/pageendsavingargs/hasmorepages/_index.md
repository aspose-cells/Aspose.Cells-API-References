---
title: "PageEndSavingArgs.HasMorePages"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageEndSavingArgs. Получает или задает значение, указывающее, есть ли еще страницы для вывода. Значение по умолчанию — true"
type: docs
url: /ru/net/aspose.cells.rendering/pageendsavingargs/hasmorepages/
---
## PageEndSavingArgs.HasMorePages property

Получает или задает значение, указывающее, есть ли ещё страницы для вывода. Значение по умолчанию — true.

```csharp
public bool HasMorePages { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageEndSavingArgsPropertyHasMorePagesDemo
    {
        public static void Run()
        {
            // Создать книгу с данными, охватывающими несколько страниц
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[i, 0].Value = $"Row {i + 1}";
            }

            // Создать параметры сохранения PDF с пользовательской обработкой страниц
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new PageControlCallback();

            // Сохранить книгу с ограничением количества страниц
            workbook.Save("PropertyHasMorePagesDemo.pdf", saveOptions);
        }
    }

    internal class PageControlCallback : IPageSavingCallback
    {
        private int pageCount = 0;

        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Не используется в этой демонстрации
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Прочитать текущее значение свойства
            Console.WriteLine($"Page {pageCount} - Initial HasMorePages: {args.HasMorePages}");

            // Изменить свойство после первой страницы
            if (pageCount == 0)
            {
                args.HasMorePages = false;
                Console.WriteLine($"Page {pageCount} - Updated HasMorePages: {args.HasMorePages}");
            }

            pageCount++;
        }
    }
}
```

### См. также

* class [PageEndSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


