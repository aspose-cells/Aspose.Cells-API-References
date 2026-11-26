---
title: "Класс PageSavingArgs"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Rendering.PageSavingArgs. Информация о процессе сохранения страницы"
type: docs
url: /ru/net/aspose.cells.rendering/pagesavingargs/
---
## PageSavingArgs class

Информация о процессе сохранения страницы.

```csharp
public class PageSavingArgs
```

## Свойства

| Имя | Описание |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Общее количество страниц. |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Текущий индекс страницы, начиная с нуля. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassPageSavingArgsDemo
    {
        public static void Run()
        {
            // Создать новую книгу с расширенными данными для нескольких страниц
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполнить лист для генерации нескольких страниц при рендеринге
            for (int row = 0; row < 150; row++)
            {
                worksheet.Cells[row, 0].Value = $"Row {row + 1} data";
            }

            // Настроить параметры сохранения PDF с обратным вызовом сохранения страниц
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.PageSavingCallback = new PageSavingCallback();

            // Сохранить книгу в формате PDF с разбиением на страницы
            workbook.Save("RenderingPageSavingDemo.pdf", pdfSaveOptions);
        }

        private class PageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                Console.WriteLine($"Saving page {args.PageIndex + 1} of {args.PageCount}");
                
                if (args.PageIndex == 0)
                {
                    Console.WriteLine("Processing cover page...");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Опционально: Добавьте любую обработку в конце страницы здесь
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


