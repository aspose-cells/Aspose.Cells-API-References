---
title: "Interface IPageSavingCallback"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Rendering.IPageSavingCallback interface. Контроль/индикация прогресса процесса сохранения страниц"
type: docs
url: /ru/net/aspose.cells.rendering/ipagesavingcallback/
---
## IPageSavingCallback interface

Управление/индикация прогресса процесса сохранения страницы.

```csharp
public interface IPageSavingCallback
```

## Методы

| Имя | Описание |
| --- | --- |
| [PageEndSaving](../../aspose.cells.rendering/ipagesavingcallback/pageendsaving/)(PageEndSavingArgs) | Контролировать/индицировать завершение вывода страницы. |
| [PageStartSaving](../../aspose.cells.rendering/ipagesavingcallback/pagestartsaving/)(PageStartSavingArgs) | Контролировать/индицировать начало вывода страницы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageSavingCallbackDemo : IPageSavingCallback
    {
        public static void PageSavingCallbackExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Создать параметры сохранения с обратным вызовом сохранения страницы
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.PageSavingCallback = new PageSavingCallbackDemo();

            // Сохранить книгу в формате DOCX
            workbook.Save("PageSavingCallbackExample.docx", saveOptions);
        }

        // Реализовать метод PageStartSaving
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex}");
        }

        // Реализовать метод PageEndSaving
        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex}");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


