---
title: "ShapeCollection.DeleteInRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Удалить фигуры в диапазоне. Комментарии фигур не будут удалены"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/deleteinrange/
---
## ShapeCollection.DeleteInRange method

Удалить фигуры в диапазоне. Фигуры‑комментарии не будут удалены.

```csharp
public void DeleteInRange(CellArea ca)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | CellArea | Диапазон. Если фигуры находятся в диапазоне, они будут удалены. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodDeleteInRangeWithCellAreaDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Добавить первую форму прямоугольника
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            // Добавить вторую форму прямоугольника
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Определить диапазон, в котором следует удалить фигуры
            CellArea area = new CellArea();
            area.StartColumn = 0;
            area.StartRow = 5;
            area.EndColumn = 5;
            area.EndRow = 8;

            // Удалить фигуры в указанном диапазоне
            shapes.DeleteInRange(area);

            // Сохраните книгу (необязательно)
            workbook.Save("ShapeDeleteInRangeDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


