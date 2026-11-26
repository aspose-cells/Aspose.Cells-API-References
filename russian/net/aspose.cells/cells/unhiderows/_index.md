---
title: "Cells.UnhideRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Делает скрытые строки видимыми"
type: docs
url: /ru/net/aspose.cells/cells/unhiderows/
---
## Cells.UnhideRows method

Отображает скрытые строки.

```csharp
public void UnhideRows(int row, int totalRows, double height)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| totalRows | Int32 | Номер строки. |
| высота | Double | Высота строки. Высота строки будет изменена только когда строка скрыта и заданное значение высоты положительно. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideRowsWithInt32Int32DoubleDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Скрыть строки 0‑4
            cells.HideRows(0, 5);
            
            // Сделать видимыми строки 0‑4 с коррекцией высоты (-1 для автоподгонки)
            cells.UnhideRows(0, 5, -1);
            
            // Проверить, что строки раскрыты
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Row {i} hidden status: {cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


