---
title: "Range.MoveTo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Переместите текущий диапазон в целевой диапазон"
type: docs
url: /ru/net/aspose.cells/range/moveto/
---
## Range.MoveTo method

Перемещает текущий диапазон в целевой диапазон.

```csharp
public void MoveTo(int destRow, int destColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destRow | Int32 | Начальная строка целевого диапазона. |
| destColumn | Int32 | Начальный столбец целевого диапазона. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodMoveToWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте пример диапазона (A1:B2)
            Aspose.Cells.Range originalRange = worksheet.Cells.CreateRange("A1", "B2");
            
            // Поместите некоторые данные в диапазон для демонстрации
            originalRange[0, 0].PutValue("A1");
            originalRange[0, 1].PutValue("B1");
            originalRange[1, 0].PutValue("A2");
            originalRange[1, 1].PutValue("B2");
            
            // Переместите диапазон вниз на 1 строку (к A2:B3)
            originalRange.MoveTo(originalRange.FirstRow + 1, originalRange.FirstColumn);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


