---
title: "Cells.CheckColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает элемент Column или null по указанному индексу столбца"
type: docs
url: /ru/net/aspose.cells/cells/checkcolumn/
---
## Cells.CheckColumn method

Получает элемент [`Column`](../../column/) или null по указанному индексу столбца.

```csharp
public Column CheckColumn(int columnIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | Int32 | Индекс столбца. |

### Возвращаемое значение

Объект Column.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckColumnWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Установить значение в столбце 1 (B3)
            cells["B3"].PutValue("Sample Data");
            
            // Проверьте столбец 4 (столбец E)
            Column column = cells.CheckColumn(4);
            
            // Вывести свойства столбца
            Console.WriteLine("Column Width: " + column.Width);
            Console.WriteLine("Column Index: " + column.Index);
        }
    }
}
```

### См. также

* class [Column](../../column/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


