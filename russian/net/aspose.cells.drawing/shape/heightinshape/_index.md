---
title: "Shape.HeightInShape"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет вертикальное смещение фигуры от верхней границы родительской фигуры в единицах 1/4000 высоты родительской фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/heightinshape/
---
## Shape.HeightInShape property

Представляет вертикальное смещение фигуры от верхней границы родительской фигуры в единицах 1/4000 высоты родительской фигуры.

```csharp
public int HeightInShape { get; set; }
```

### Примечания

Применяется только когда эта фигура находится в группе или диаграмме.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightInShapeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Сначала добавьте формы со всеми необходимыми параметрами
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 10, 10);
            Shape oval = worksheet.Shapes.AddOval(0, 0, 100, 100, 10, 120);

            // Сгруппировать фигуры
            Shape[] shapes = { rectangle, oval };
            GroupShape groupShape = worksheet.Shapes.Group(shapes);

            // Установите высоту прямоугольника относительно родительской групповой формы (1/4000 от высоты родителя)
            rectangle.HeightInShape = 2000; // Half the height of the parent
            oval.HeightInShape = 4000; // Full height of the parent

            // Сохраните книгу
            workbook.Save("ShapeHeightInShapeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


