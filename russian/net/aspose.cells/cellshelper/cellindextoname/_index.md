---
title: "CellsHelper.CellIndexToName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsHelper. Получает имя ячейки в соответствии с её строкой и столбцовыми индексами"
type: docs
url: /ru/net/aspose.cells/cellshelper/cellindextoname/
---
## CellsHelper.CellIndexToName method

Получает имя ячейки в соответствии с её индексами строки и столбца.

```csharp
public static string CellIndexToName(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| column | Int32 | Индекс столбца. |

### Возвращаемое значение

Имя ячейки.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCellIndexToNameWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните некоторыми данными
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(20);

            // Получить имя ячейки по индексам строки и столбца
            string cellName = CellsHelper.CellIndexToName(2, 1); // Row 2, Column 1 (B3)

            // Вывести результат.
            Console.WriteLine("Cell name for row 2, column 1 is: " + cellName);
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


