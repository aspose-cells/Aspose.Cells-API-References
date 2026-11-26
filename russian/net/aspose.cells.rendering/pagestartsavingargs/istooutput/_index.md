---
title: "PageStartSavingArgs.IsToOutput"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageStartSavingArgs. Получает или задает значение, указывающее, следует ли выводить страницу. Значение по умолчанию — true"
type: docs
url: /ru/net/aspose.cells.rendering/pagestartsavingargs/istooutput/
---
## PageStartSavingArgs.IsToOutput property

Получает или задаёт значение, указывающее, должна ли страница выводиться. Значение по умолчанию — true.

```csharp
public bool IsToOutput { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageStartSavingArgsPropertyIsToOutputDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните данные, чтобы создать несколько страниц
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
                // Исправлено: доступ к высоте строки через коллекцию Rows листа
                worksheet.Cells.Rows[i].Height = 50;
            }

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new CustomPageSavingCallback();

            workbook.Save("PageOutputDemo.pdf", saveOptions);
        }

        private class CustomPageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Прочитать текущее значение
                Console.WriteLine($"Page {args.PageIndex + 1} - Initial IsToOutput: {args.IsToOutput}");

                // Пропускать каждую четную страницу (нумерация с 1)
                if ((args.PageIndex + 1) % 2 == 0)
                {
                    args.IsToOutput = false;
                    Console.WriteLine($"Disabling output for page {args.PageIndex + 1}");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Реализация не требуется для этой демонстрации
            }
        }
    }
}
```

### См. также

* class [PageStartSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


