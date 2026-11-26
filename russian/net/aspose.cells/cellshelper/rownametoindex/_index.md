---
title: "CellsHelper.RowNameToIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsHelper. Получает индекс строки по имени строки"
type: docs
url: /ru/net/aspose.cells/cellshelper/rownametoindex/
---
## CellsHelper.RowNameToIndex method

Получает индекс строки в соответствии с её именем.

```csharp
public static int RowNameToIndex(string rowName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowName | String | Имя строки. |

### Возвращаемое значение

Индекс строки.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodRowNameToIndexWithStringDemo
    {
        public static void Run()
        {
            string rowName = "11";
            int rowIndex = CellsHelper.RowNameToIndex(rowName);
            Console.WriteLine("Row name '{0}' converted to index: {1}", rowName, rowIndex);
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


