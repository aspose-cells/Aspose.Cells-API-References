---
title: "ShapeCollection.Group"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Группировать фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/group/
---
## ShapeCollection.Group method

Группировать фигуры.

```csharp
public GroupShape Group(Shape[] groupItems)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| groupItems | Shape[] | элементы группы. |

### Возвращаемое значение

Возвращает форму группы.

### Примечания

Форма в groupItems не должна быть сгруппирована. Форма должна находиться в этой коллекции Shapes.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodGroupWithShapeArrayDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить коллекцию фигур
            ShapeCollection shapes = worksheet.Shapes;

            // Добавить первую форму прямоугольника
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Добавить вторую форму прямоугольника
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Создайте массив с формами для группировки
            Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };

            // Сгруппировать фигуры
            GroupShape groupShape = shapes.Group(shapesArr);

            // Сохраните книгу
            workbook.Save("GroupShapesDemo.xlsx");
        }
    }
}
```

### См. также

* class [GroupShape](../../groupshape/)
* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


