---
title: "WorksheetCollection.CreateRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorksheetCollection. Создаёт объект Range из адреса диапазона"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/createrange/
---
## WorksheetCollection.CreateRange method

Создаёт объект [`Range`](../../range/) из адреса диапазона.

```csharp
public Range CreateRange(string address, int sheetIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| address | String | Адрес диапазона. |
| sheetIndex | Int32 | Индекс листа. |

### Возвращаемое значение

Объект [`Range`](../../range/)

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodCreateRangeWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните некоторыми образцовыми данными
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 6; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            // Создать диапазон, используя строковый адрес и индекс листа
            Aspose.Cells.Range range = workbook.Worksheets.CreateRange("A1:F10", 0);

            // Продемонстрировать использование диапазона
            Console.WriteLine($"Range has {range.RowCount} rows and {range.ColumnCount} columns");
            Console.WriteLine($"First cell value: {range[0, 0].StringValue}");
            Console.WriteLine($"Last cell value: {range[9, 5].StringValue}");
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


