---
title: "PaginatedSaveOptions.PageSavingCallback"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Управляет/отображает прогресс процесса сохранения страниц"
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/pagesavingcallback/
---
## PaginatedSaveOptions.PageSavingCallback property

Управление/индикация прогресса процесса сохранения страницы.

```csharp
public IPageSavingCallback PageSavingCallback { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageSavingCallbackDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            worksheet.Cells["A2"].PutValue("This demonstrates PageSavingCallback");

            // Создайте параметры сохранения с обратным вызовом сохранения страниц
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new CustomPageSavingCallback();

            // Сохранить с обратным вызовом
            workbook.Save("PageSavingCallbackDemo.pdf", saveOptions);
        }
    }

    public class CustomPageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex + 1}");
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex + 1}");
            if (args.HasMorePages)
            {
                Console.WriteLine("More pages to follow...");
            }
        }
    }
}
```

### См. также

* interface [IPageSavingCallback](../../../aspose.cells.rendering/ipagesavingcallback/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


