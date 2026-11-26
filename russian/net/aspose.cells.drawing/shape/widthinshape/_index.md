---
title: "Shape.WidthInShape"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет ширину фигуры в единице 1/4000 от родительской фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/widthinshape/
---
## Shape.WidthInShape property

Представляет ширину фигуры, в единицах 1/4000 от родительской фигуры.

```csharp
public int WidthInShape { get; set; }
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
    public class ShapePropertyWidthInShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать две прямоугольные фигуры
            Shape rect1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            Shape rect2 = worksheet.Shapes.AddRectangle(0, 100, 0, 0, 100, 100);
            
            // Группировать фигуры, используя объекты Shape
            GroupShape group = worksheet.Shapes.Group(new Shape[] { rect1, rect2 });
            
            // Продемонстрировать использование WidthInShape
            if (rect1.IsInGroup && rect1.WidthInShape == 2000)
            {
                rect1.WidthInShape = 4000;
            }
            
            // Сохранить изменённую книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


