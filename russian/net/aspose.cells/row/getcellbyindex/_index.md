---
title: "Row.GetCellByIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Row. Получить ячейку по конкретному индексу в коллекции ячеек этой строки"
type: docs
url: /ru/net/aspose.cells/row/getcellbyindex/
---
## Row.GetCellByIndex method

Получить ячейку по конкретному индексу в коллекции ячеек этой строки.

```csharp
public Cell GetCellByIndex(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс (позиция) ячейки в коллекции ячеек этой строки. |

### Возвращаемое значение

Объект Cell в заданной позиции.

### Примечания

Для последовательного обхода всех ячеек без изменения использование [`GetEnumerator`](../getenumerator/) даст лучшую производительность, чем использование этого метода для получения ячеек по одной.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetCellByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить данные в ячейки первой строки
            worksheet.Cells["A1"].PutValue("Cell A1");
            worksheet.Cells["B1"].PutValue("Cell B1");
            worksheet.Cells["C1"].PutValue("Cell C1");

            // Получить первую строку
            Row row = worksheet.Cells.Rows[0];

            // Продемонстрировать GetCellByIndex с параметром Int32
            Cell cellAtIndex0 = row.GetCellByIndex(0);
            Cell cellAtIndex1 = row.GetCellByIndex(1);
            Cell cellAtIndex2 = row.GetCellByIndex(2);

            Console.WriteLine("Cell at index 0: " + cellAtIndex0.StringValue);
            Console.WriteLine("Cell at index 1: " + cellAtIndex1.StringValue);
            Console.WriteLine("Cell at index 2: " + cellAtIndex2.StringValue);

            workbook.Save("RowGetCellByIndexDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


