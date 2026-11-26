---
title: "CellsHelper.ColumnNameToIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsHelper. Получает индекс столбца по имени столбца"
type: docs
url: /ru/net/aspose.cells/cellshelper/columnnametoindex/
---
## CellsHelper.ColumnNameToIndex method

Получает индекс столбца в соответствии с именем столбца.

```csharp
public static int ColumnNameToIndex(string columnName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnName | String | Имя столбца. |

### Возвращаемое значение

Индекс столбца.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodColumnNameToIndexWithStringDemo
    {
        public static void Run()
        {
            int columnIndex = CellsHelper.ColumnNameToIndex("BAA");
            string columnName = CellsHelper.ColumnIndexToName(columnIndex);
            
            Console.WriteLine("Column Name: " + columnName);
            Console.WriteLine("Column Index: " + columnIndex);
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


