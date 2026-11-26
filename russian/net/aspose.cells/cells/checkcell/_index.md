---
title: "Cells.CheckCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает элемент Cell или null по указанному индексу строки и столбца ячейки"
type: docs
url: /ru/net/aspose.cells/cells/checkcell/
---
## Cells.CheckCell method

Получает элемент [`Cell`](../../cell/) или null по указанному индексу строки и столбца ячейки.

```csharp
public Cell CheckCell(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки |
| column | Int32 | Индекс столбца |

### Возвращаемое значение

Возвращает объект Cell, если он существует. Возвращает null, если ячейка не существует.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckCellWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить значения в cells
            cells[0, 0].PutValue("Hello");
            cells[1, 1].PutValue(123);
            cells[2, 2].PutValue(DateTime.Now);

            // Проверить ячейки, используя метод CheckCell с параметрами типа Int32
            Cell cell1 = cells.CheckCell(0, 0);
            Console.WriteLine("Cell A1 value: " + cell1.StringValue);

            Cell cell2 = cells.CheckCell(1, 1);
            Console.WriteLine("Cell B2 value: " + cell2.StringValue);

            Cell cell3 = cells.CheckCell(2, 2);
            Console.WriteLine("Cell C3 value: " + cell3.StringValue);

            // Проверить несуществующую ячейку (вернёт null)
            Cell cell4 = cells.CheckCell(10, 10);
            if (cell4 == null)
            {
                Console.WriteLine("Cell K11 doesn't exist (as expected)");
            }
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


