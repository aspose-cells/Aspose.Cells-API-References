---
title: "Worksheet.IsRulerVisible"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Указывает, видима ли линейка. Это свойство применяется только в режиме предварительного просмотра разрывов страниц"
type: docs
url: /ru/net/aspose.cells/worksheet/isrulervisible/
---
## Worksheet.IsRulerVisible property

Указывает, видима ли линейка. Это свойство применяется только в режиме предварительного просмотра разрывов страниц.

```csharp
public bool IsRulerVisible { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsRulerVisibleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить лист в режим PageLayoutView, где линейка видима
            worksheet.ViewType = ViewType.PageLayoutView;

            // Переключить видимость линейки
            worksheet.IsRulerVisible = true;

            // Вывести текущее состояние видимости линейки
            Console.WriteLine("Worksheet ruler is visible: " + worksheet.IsRulerVisible);

            // Сохраните книгу
            workbook.Save("WorksheetRulerVisibilityDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


