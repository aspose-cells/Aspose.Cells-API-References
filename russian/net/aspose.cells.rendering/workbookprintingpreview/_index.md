---
title: "Класс WorkbookPrintingPreview"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Rendering.WorkbookPrintingPreview класс. Предпросмотр печати книги"
type: docs
url: /ru/net/aspose.cells.rendering/workbookprintingpreview/
---
## WorkbookPrintingPreview class

Предпросмотр печати книги.

```csharp
public class WorkbookPrintingPreview
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WorkbookPrintingPreview](workbookprintingpreview/)(Workbook, ImageOrPrintOptions) | Конструктор WorkbookPrintingPreview |

## Свойства

| Имя | Описание |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/) { get; } | Оцените общее количество страниц этой рабочей книги |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class WorkbookPrintingPreviewDemo
    {
        public static void WorkbookPrintingPreviewExample()
        {
            // Загрузите существующую книгу
            Workbook workbook = new Workbook("WorkbookPrintingPreviewExample_original.xlsx");

            // Создайте экземпляр ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Создайте экземпляр WorkbookPrintingPreview
            WorkbookPrintingPreview workbookPrintingPreview = new WorkbookPrintingPreview(workbook, options);

            // Оцените общее количество страниц рабочей книги
            int pageCount = workbookPrintingPreview.EvaluatedPageCount;

            // Выведите оценённое количество страниц
            Console.WriteLine("Total Page Count: " + pageCount);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


