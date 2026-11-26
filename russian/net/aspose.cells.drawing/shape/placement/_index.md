---
title: "Shape.Placement"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет способ, которым объект рисунка привязан к ячейкам под ним. Свойство управляет размещением объекта на листе."
type: docs
url: /ru/net/aspose.cells.drawing/shape/placement/
---
## Shape.Placement property

Представляет способ, которым объект рисунка прикреплен к находящимся под ним ячейкам. Свойство управляет размещением объекта на листе.

```csharp
public PlacementType Placement { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyPlacementDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 50);

            // Продемонстрировать свойство Placement
            Console.WriteLine("Original Placement: " + shape.Placement);
            
            // Измените тип размещения
            shape.Placement = PlacementType.MoveAndSize;
            Console.WriteLine("Modified Placement: " + shape.Placement);

            // Сохраните книгу
            workbook.Save("ShapePlacementDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PlacementType](../../placementtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


