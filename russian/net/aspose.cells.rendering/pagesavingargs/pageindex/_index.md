---
title: "PageSavingArgs.PageIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSavingArgs. Текущий индекс страницы, начиная с нуля"
type: docs
url: /ru/net/aspose.cells.rendering/pagesavingargs/pageindex/
---
## PageSavingArgs.PageIndex property

Текущий индекс страницы, начиная с нуля.

```csharp
public int PageIndex { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSavingArgsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить некоторые данные в лист
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // Создайте параметры сохранения PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Установите обратный вызов сохранения страницы
            options.PageSavingCallback = new PageSavingCallback();

            // Сохраните книгу в PDF — это вызовет обратный вызов для каждой страницы
            workbook.Save("output.pdf", options);
        }
    }

    public class PageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Продемонстрируйте использование свойства PageIndex
            Console.WriteLine($"Starting to save page {args.PageIndex + 1}");
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Не используется в этом примере
        }
    }
}
```

### См. также

* class [PageSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


