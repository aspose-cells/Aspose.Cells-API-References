---
title: "Класс SheetPrintingPreview"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Rendering.SheetPrintingPreview. Предпросмотр печати листа"
type: docs
url: /ru/net/aspose.cells.rendering/sheetprintingpreview/
---
## SheetPrintingPreview class

Предпросмотр печати листа.

```csharp
public class SheetPrintingPreview
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SheetPrintingPreview](sheetprintingpreview/)(Worksheet, ImageOrPrintOptions) | Конструкция SheetPrintingPreview |

## Свойства

| Имя | Описание |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/sheetprintingpreview/evaluatedpagecount/) { get; } | Оцените общее количество страниц этого листа |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetPrintingPreviewDemo
    {
        public static void SheetPrintingPreviewExample()
        {
            // Загрузите существующую книгу
            Workbook workbook = new Workbook("SheetPrintingPreviewDemo_original.xlsx");

            // Получить первый лист
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте экземпляр ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Создайте экземпляр SheetPrintingPreview
            SheetPrintingPreview sheetPrintingPreview = new SheetPrintingPreview(worksheet, options);

            // Оцените и выведите общее количество страниц листа
            Console.WriteLine("Total Page Count: " + sheetPrintingPreview.EvaluatedPageCount);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


