---
title: "Cells.AddRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Добавляет ссылку на объект диапазона в ячейки"
type: docs
url: /ru/net/aspose.cells/cells/addrange/
---
## Cells.AddRange method

Добавляет ссылку на объект диапазона в ячейки

```csharp
public void AddRange(Range rangeObject)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rangeObject | Диапазон | Объект диапазона будет содержаться в ячейках |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodAddRangeWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите примерные данные в диапазоне
            cells["A1"].PutValue("A1");
            cells["A2"].PutValue("A2");
            cells["B1"].PutValue("B1");
            cells["B2"].PutValue("B2");

            // Создайте диапазон и добавьте его с помощью AddRange
            Aspose.Cells.Range range = cells.CreateRange("A1", "B2");
            cells.AddRange(range);

            // Измените лист, чтобы продемонстрировать расширение диапазона
            cells.InsertRow(1);
            cells.InsertColumn(1);

            Console.WriteLine($"Range now has {range.RowCount} rows and {range.ColumnCount} columns");
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


