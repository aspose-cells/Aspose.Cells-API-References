---
title: "Row.GetCellOrNull"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Row. Получает ячейку или null по конкретному индексу"
type: docs
url: /ru/net/aspose.cells/row/getcellornull/
---
## Row.GetCellOrNull method

Получает ячейку или null по указанному индексу.

```csharp
public Cell GetCellOrNull(int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца |

### Возвращаемое значение

Возвращает объект ячейки, если ячейка существует. Или возвращает null, если объект ячейки не существует.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetCellOrNullWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Добавьте примерные данные
            ws.Cells["A1"].PutValue("Header1");
            ws.Cells["B1"].PutValue("Header2");
            ws.Cells["A2"].PutValue(100);
            ws.Cells["B2"].PutValue(200);

            // Получить первую строку
            Row row = ws.Cells.Rows[0];

            // Продемонстрировать GetCellOrNull с параметром Int32
            for (int colIndex = 0; colIndex < 2; colIndex++)
            {
                Cell cell = row.GetCellOrNull(colIndex);
                if (cell != null)
                {
                    Console.WriteLine($"Cell at column {colIndex}: {cell.StringValue}");
                }
                else
                {
                    Console.WriteLine($"Cell at column {colIndex} is null");
                }
            }
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


