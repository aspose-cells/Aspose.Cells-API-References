---
title: "ErrorCheckOptionCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "ErrorCheckOptionCollection свойство. Получает объект ErrorCheckOption по заданному индексу"
type: docs
url: /ru/net/aspose.cells/errorcheckoptioncollection/item/
---
## ErrorCheckOptionCollection indexer

Получает объект [`ErrorCheckOption`](../../errorcheckoption/) по заданному индексу.

```csharp
public ErrorCheckOption this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс |

### Возвращаемое значение

Вернуть объект [`ErrorCheckOption`](../../errorcheckoption/)

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ErrorCheckOptionCollection opts = worksheet.ErrorCheckOptions;
            int optionIdx = opts.Add();
            
            // Продемонстрировать использование свойства Item
            ErrorCheckOption opt = opts[optionIdx];
            
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.AddRange(CellArea.CreateCellArea("A1", "B3"));

            workbook.Save("ErrorCheckOptionDemo.xlsx");
        }
    }
}
```

### См. также

* class [ErrorCheckOption](../../errorcheckoption/)
* class [ErrorCheckOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


