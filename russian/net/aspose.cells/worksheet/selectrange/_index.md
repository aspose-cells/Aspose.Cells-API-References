---
title: "Worksheet.SelectRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Выбирает диапазон"
type: docs
url: /ru/net/aspose.cells/worksheet/selectrange/
---
## Worksheet.SelectRange method

Выбирает диапазон.

```csharp
public void SelectRange(int startRow, int startColumn, int totalRows, int totalColumns, 
    bool removeOthers)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Начальная строка. |
| startColumn | Int32 | Начальный столбец |
| totalRows | Int32 | Количество строк. |
| totalColumns | Int32 | Количество столбцов |
| removeOthers | Boolean | True означает удаление других выбранных диапазонов и выбор только этого диапазона. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSelectRangeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Выбрать диапазон от строки 1, столбца 1 до строки 5, столбца 5 (B2:F6) и сделать его активным
            worksheet.SelectRange(1, 1, 5, 5, true);
            
            Console.WriteLine("Active cell: " + worksheet.ActiveCell);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


