---
title: "RangeCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод RangeCollection. Добавляет элемент Range в коллекцию"
type: docs
url: /ru/net/aspose.cells/rangecollection/add/
---
## RangeCollection.Add method

Добавляет элемент [`Range`](../../range/) в коллекцию.

```csharp
[Obsolete("Use RangeCollection.AddRange(Range) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(Range range)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| диапазон | Диапазон | Объект Range |

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод AddRange(). Этот метод будет удалён через 6 месяцев, начиная с декабря 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeCollectionMethodAddWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать диапазон и добавить его в коллекцию
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            
            // Вставить строки, чтобы продемонстрировать расширение диапазона
            worksheet.Cells.InsertRows(2, 2);
            
            Console.WriteLine("Range row count after insertion: " + cellRange.RowCount);
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


