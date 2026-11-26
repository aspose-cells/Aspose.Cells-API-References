---
title: "CellsHelper.RowIndexToName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsHelper. Получает имя строки по её индексу"
type: docs
url: /ru/net/aspose.cells/cellshelper/rowindextoname/
---
## CellsHelper.RowIndexToName method

Получает имя строки в соответствии с индексом строки.

```csharp
public static string RowIndexToName(int row)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |

### Возвращаемое значение

Имя строки.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodRowIndexToNameWithInt32Demo
    {
        public static void Run()
        {
            int rowIndex = 10;
            string rowName = CellsHelper.RowIndexToName(rowIndex);
            Console.WriteLine("Row index {0} corresponds to row name: {1}", rowIndex, rowName);
            
            int convertedBackIndex = CellsHelper.RowNameToIndex(rowName);
            Console.WriteLine("Row name {0} converted back to index: {1}", rowName, convertedBackIndex);
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


