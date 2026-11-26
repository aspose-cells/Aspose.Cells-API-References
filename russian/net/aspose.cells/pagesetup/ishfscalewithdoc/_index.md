---
title: "PageSetup.IsHFScaleWithDoc"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Указывает, масштабируются ли верхний и нижний колонтитулы вместе с масштабированием документа. Применяется только для Excel 2007"
type: docs
url: /ru/net/aspose.cells/pagesetup/ishfscalewithdoc/
---
## PageSetup.IsHFScaleWithDoc property

Указывает, масштабируются ли верхний и нижний колонтитулы вместе с масштабированием документа. Применяется только к Excel 2007.

```csharp
public bool IsHFScaleWithDoc { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFScaleWithDocDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Доступ к PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Установите базовые параметры страницы.
            pageSetup.Orientation = PageOrientationType.Landscape;
            pageSetup.PaperSize = PaperSizeType.PaperA4;

            // Продемонстрировать свойство IsHFScaleWithDoc.
            pageSetup.IsHFScaleWithDoc = true;
            Console.WriteLine("Header/Footer scaling with document is set to: " + pageSetup.IsHFScaleWithDoc);

            // Сохраните книгу
            workbook.Save("PageSetup_IsHFScaleWithDoc_Demo.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


