---
title: "Cells.MoveRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Перемещает диапазон"
type: docs
url: /ru/net/aspose.cells/cells/moverange/
---
## Cells.MoveRange method

Перемещает диапазон.

```csharp
public void MoveRange(CellArea sourceArea, int destRow, int destColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceArea | CellArea | Диапазон, который следует переместить. |
| destRow | Int32 | Строка назначения. |
| destColumn | Int32 | Столбец назначения. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMoveRangeWithCellAreaInt32Int32Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Поместить значения в ячейки
            cells["A1"].PutValue("Original");
            cells["B1"].PutValue(100);
            cells["A2"].PutValue("Data");
            cells["B2"].PutValue(200);

            // Определите область ячеек для перемещения (A1:B2)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 1;
            area.EndColumn = 1;

            // Переместите диапазон вниз на 2 строки и вправо на 3 столбца
            cells.MoveRange(area, 2, 3);

            // Сохраните книгу
            workbook.Save("MoveRangeExample.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


