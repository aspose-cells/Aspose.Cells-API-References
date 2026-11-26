---
title: "Range.GetEnumerator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Получает перечислитель для ячеек в этом диапазоне"
type: docs
url: /ru/net/aspose.cells/range/getenumerator/
---
## Range.GetEnumerator method

Получает перечислитель для ячеек в этом Range.

```csharp
public IEnumerator GetEnumerator()
```

### Возвращаемое значение

Перечислитель ячеек

### Примечания

При обходе элементов с помощью возвращённого Enumerator, коллекцию Cells не следует изменять(например, операции, которые приведут к созданию новых Cell/Row или удалению существующих Cell/Row). В противном случае перечислитель может не суметь корректно пройти все ячейки(некоторые элементы могут быть пройдены несколько раз или пропущены).

### Примеры

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполните некоторыми образцовыми данными
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Banana");
            worksheet.Cells["C2"].PutValue("Cherry");
            worksheet.Cells["C3"].PutValue("Date");

            // Получить диапазон и перечислить ячейки
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C3");
            IEnumerator enumerator = range.GetEnumerator();
            
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                Console.WriteLine($"{cell.Name}: {cell.Value}");
            }
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


