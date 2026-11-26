---
title: "Cells.CheckRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает элемент Row или null по указанному индексу строки ячейки"
type: docs
url: /ru/net/aspose.cells/cells/checkrow/
---
## Cells.CheckRow method

Получает элемент [`Row`](../../row/) или null по указанному индексу строки ячейки.

```csharp
public Row CheckRow(int row)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки |

### Возвращаемое значение

Возвращает объект [`Row`](../../row/), если объект строки существует, иначе возвращает null.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckRowWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Заполните некоторыми данными
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(100);
            cells["A3"].PutValue(200);
            
            // Проверьте, существует ли строка, и получите объект строки
            Row row = cells.CheckRow(1);
            if (row != null)
            {
                Console.WriteLine("Row 1 exists with height: " + row.Height);
            }
            
            // Проверьте несуществующую строку
            Row nonExistentRow = cells.CheckRow(100);
            Console.WriteLine("Row 100 exists: " + (nonExistentRow != null));
        }
    }
}
```

### См. также

* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


