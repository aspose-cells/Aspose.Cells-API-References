---
title: "PageSavingArgs.PageCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSavingArgs. Общее количество страниц"
type: docs
url: /ru/net/aspose.cells.rendering/pagesavingargs/pagecount/
---
## PageSavingArgs.PageCount property

Общее количество страниц.

```csharp
public int PageCount { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageSavingArgsPropertyPageCountDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и добавьте тестовые данные
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте плотное содержимое, чтобы создать несколько страниц
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            // Настройте параметры страницы для управления разбиением на страницы
            worksheet.PageSetup.PrintArea = "A1:A50";
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            // Создайте параметры сохранения PDF с обратным вызовом сохранения страницы
            PdfSaveOptions options = new PdfSaveOptions();
            options.PageSavingCallback = new PageSavingCallback();

            // Сохраните в PDF, чтобы вызвать разбиение на страницы
            workbook.Save("PageSavingDemo.pdf", options);
        }

        private class PageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Получите PageCount из аргументов события
                Console.WriteLine($"Saving page {args.PageIndex + 1} of {args.PageCount}");
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Реализация не требуется
            }
        }
    }
}
```

### См. также

* class [PageSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


