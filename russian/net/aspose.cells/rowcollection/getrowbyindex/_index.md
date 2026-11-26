---
title: "RowCollection.GetRowByIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод RowCollection. Возвращает объект строки по позиции в списке"
type: docs
url: /ru/net/aspose.cells/rowcollection/getrowbyindex/
---
## RowCollection.GetRowByIndex method

Получает объект строки по позиции в списке.

```csharp
public Row GetRowByIndex(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Позиция. |

### Возвращаемое значение

Объект Row в указанной позиции.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionMethodGetRowByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Получить строку по индексу (нумерация с нуля)
            Row row = sheet.Cells.Rows.GetRowByIndex(0);
            
            if (row == null)
            {
                Console.WriteLine("Row at index 0 is null (not created yet)");
            }
            else
            {
                Console.WriteLine("Row at index 0 exists");
            }
        }
    }
}
```

### См. также

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


