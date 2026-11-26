---
title: "ShapeCollection.Ungroup"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Разъединяет элементы фигур"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/ungroup/
---
## ShapeCollection.Ungroup method

Разгруппировать элементы фигуры.

```csharp
public void Ungroup(GroupShape group)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| группа | GroupShape | Групповая фигура. |

### Примечания

Если групповая фигура сгруппирована другой групповой фигурой, ничего не будет сделано.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodUngroupWithGroupShapeDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить коллекцию фигур
            ShapeCollection shapes = worksheet.Shapes;

            // Добавить первую форму прямоугольника
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Добавить вторую форму прямоугольника
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Создайте массив фигур для группировки
            Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };

            // Сгруппировать фигуры
            GroupShape groupShape = shapes.Group(shapesArr);

            // Разъединить групповую фигуру
            shapes.Ungroup(groupShape);
        }
    }
}
```

### См. также

* class [GroupShape](../../groupshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


