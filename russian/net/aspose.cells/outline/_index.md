---
title: "Класс Outline"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Outline. Представляет outline на листе"
type: docs
url: /ru/net/aspose.cells/outline/
---
## Outline class

Представляет структуру на листе.

```csharp
public class Outline
```

## Свойства

| Имя | Описание |
| --- | --- |
| [SummaryColumnRight](../../aspose.cells/outline/summarycolumnright/) { get; set; } | Указывает, будет ли столбец итогов размещён справа от столбцов деталей в outline. |
| [SummaryRowBelow](../../aspose.cells/outline/summaryrowbelow/) { get; set; } | Указывает, будет ли строка итогов размещена ниже строк деталей в outline. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OutlineDemo
    {
        public static void OutlineExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу в рабочей книге
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получите доступ к outline листа
            Outline outline = worksheet.Outline;
            
            // Установите свойства outline
            outline.SummaryRowBelow = true; // Indicates if the summary row will be positioned below the detail rows
            outline.SummaryColumnRight = true; // Indicates if the summary column will be positioned to the right of the detail columns
            
            // Сохраните книгу
            workbook.Save("OutlineExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


