---
title: "Cells.GetEnumerator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает перечислитель ячеек"
type: docs
url: /ru/net/aspose.cells/cells/getenumerator/
---
## Cells.GetEnumerator method

Получает перечислитель ячеек.

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
    public class CellsMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            
            // Получите перечислитель и пройдите ячейки
            IEnumerator enumerator = worksheet.Cells.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                if (cell.Value != null)
                {
                    Console.WriteLine($"{cell.Name}: {cell.Value}");
                }
            }
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


