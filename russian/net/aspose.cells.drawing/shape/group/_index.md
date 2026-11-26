---
title: "Shape.Group"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает групповую фигуру, содержащую эту фигуру"
type: docs
url: /ru/net/aspose.cells.drawing/shape/group/
---
## Shape.Group property

Получает групповую фигуру, содержащую эту фигуру.

```csharp
public GroupShape Group { get; }
```

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyGroupDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создать две примерные фигуры
            Shape shape1 = sheet.Shapes.AddRectangle(0, 0, 0, 100, 100, 0);
            Shape shape2 = sheet.Shapes.AddOval(0, 100, 100, 100, 100, 0);

            // Сгруппировать фигуры, используя параметр массива Shape
            GroupShape group = sheet.Shapes.Group(new Shape[] { shape1, shape2 });

            // Получить доступ к группе через свойство Group дочерней фигуры
            GroupShape retrievedGroup = shape1.Group;
            
            // Продемонстрировать использование свойства Group
            retrievedGroup.Name = "MyShapeGroup";
            retrievedGroup.Placement = PlacementType.FreeFloating;

            workbook.Save("GroupShapeDemo.xlsx");
        }
    }
}
```

### См. также

* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


