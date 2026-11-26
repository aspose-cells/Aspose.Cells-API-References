---
title: "Перечисление PrintOrderType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.PrintOrderType. Представляет константы порядка печати"
type: docs
url: /ru/net/aspose.cells/printordertype/
---
## PrintOrderType enumeration

Представляет константы порядка печати.

```csharp
public enum PrintOrderType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| DownThenOver | `0` | Вниз, затем вправо |
| OverThenDown | `1` | Вправо, затем вниз |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintOrderTypeDemo
    {
        public static void PrintOrderTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Доступ к объекту PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Установить порядок печати в DownThenOver
            pageSetup.Order = PrintOrderType.DownThenOver;

            // Установить некоторые другие свойства настройки страницы для демонстрации
            pageSetup.PrintArea = "A1:D10";
            pageSetup.PrintTitleRows = "$1:$1";
            pageSetup.PrintTitleColumns = "$A:$A";
            pageSetup.CenterHorizontally = true;
            pageSetup.CenterVertically = true;

            // Сохраните книгу
            workbook.Save("PrintOrderTypeExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


