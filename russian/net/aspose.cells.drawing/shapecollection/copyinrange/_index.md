---
title: "ShapeCollection.CopyInRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Копирует фигуры из диапазона в целевой диапазон"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/copyinrange/
---
## ShapeCollection.CopyInRange method

Скопировать фигуры в диапазоне в целевой диапазон.

```csharp
public void CopyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, 
    bool isContained)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceShapes | ShapeCollection | Исходные фигуры. |
| ca | CellArea | Исходный диапазон. |
| destRow | Int32 | Индекс строки назначения в целевом диапазоне. |
| destColumn | Int32 | Столбец назначения в целевом диапазоне. |
| isContained | Boolean | Определяет, копировать ли только фигуры, находящиеся в диапазоне. Если true, копирует только фигуры в диапазоне. В противном случае работает как MS Office. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodCopyInRangeWithShapeCollectionCellAreaInt32InDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить коллекцию фигур
            ShapeCollection shapes = worksheet.Shapes;

            // Добавить прямоугольную фигуру
            shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Определите область ячеек для копирования.
            CellArea area2 = new CellArea();
            area2.StartColumn = 1;
            area2.StartRow = 1;
            area2.EndColumn = 5;
            area2.EndRow = 11;

            // Копировать фигуры в указанном диапазоне.
            shapes.CopyInRange(shapes, area2, 12, 1, false);

            // Сохраните книгу
            workbook.Save("ShapeCopyDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


