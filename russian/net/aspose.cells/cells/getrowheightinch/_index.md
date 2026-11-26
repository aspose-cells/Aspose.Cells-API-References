---
title: "Cells.GetRowHeightInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает высоту указанной строки в единицах дюймов"
type: docs
url: /ru/net/aspose.cells/cells/getrowheightinch/
---
## Cells.GetRowHeightInch method

Получает высоту указанной строки в дюймах.

```csharp
public double GetRowHeightInch(int row)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки |

### Возвращаемое значение

Высота строки

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightInchWithInt32Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить высоту строки в дюймах для строки 5
            cells.SetRowHeightInch(5, 1.5);

            // Получить высоту строки в дюймах для строки 5
            double rowHeight = cells.GetRowHeightInch(5);

            // Вывести результат.
            Console.WriteLine("Row height in inches: " + rowHeight);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


