---
title: "ShapeCollection.Remove"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Удалить форму"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/remove/
---
## ShapeCollection.Remove method

Удалить фигуру.

```csharp
public void Remove(Shape shape)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| фигура | Фигура |  |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodRemoveWithShapeDemo
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

            // Получить первую фигуру по имени или индексу
            Shape shapeToRemove = shapes["Rectangle 1"]; // or shapes[0];
            
            if (shapeToRemove != null)
            {
                // Удалить фигуру из коллекции
                shapes.Remove(shapeToRemove);
            }

            // Сохраните книгу
            workbook.Save("ShapeRemoveDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


