---
title: "Shape.IsInGroup"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Указывает, сгруппирована ли форма"
type: docs
url: /ru/net/aspose.cells.drawing/shape/isingroup/
---
## Shape.IsInGroup property

Указывает, сгруппирована ли фигура.

```csharp
public bool IsInGroup { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyIsInGroupDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте несколько форм с указанием всех необходимых параметров (upperLeftRow, upperLeftColumn, height, width, imageWidth, imageHeight)
            Shape shape1 = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 50, 100);
            Shape shape2 = worksheet.Shapes.AddRectangle(6, 0, 2, 0, 50, 100);
            Shape shape3 = worksheet.Shapes.AddRectangle(3, 0, 5, 0, 50, 100);

            // Сгруппируйте формы с правильными параметрами
            GroupShape group = worksheet.Shapes.Group(new Shape[] { shape1, shape2, shape3 });

            // Проверьте, находятся ли формы в группе
            Console.WriteLine("Shape1 IsInGroup: " + shape1.IsInGroup);
            Console.WriteLine("Shape2 IsInGroup: " + shape2.IsInGroup);
            Console.WriteLine("Shape3 IsInGroup: " + shape3.IsInGroup);
            Console.WriteLine("GroupShape IsInGroup: " + group.IsInGroup);

            // Добавьте форму без группировки
            Shape ungroupedShape = worksheet.Shapes.AddRectangle(10, 0, 2, 0, 50, 100);
            Console.WriteLine("Ungrouped shape IsInGroup: " + ungroupedShape.IsInGroup);

            // Сохранить результат
            workbook.Save("ShapePropertyIsInGroupDemo.xlsx");

            // Разгруппируйте формы и получите разгруппированные формы из группы
            group.Ungroup();
            Console.WriteLine("After ungrouping, shape1 IsInGroup: " + shape1.IsInGroup);
            Console.WriteLine("After ungrouping, shape2 IsInGroup: " + shape2.IsInGroup);
            Console.WriteLine("After ungrouping, shape3 IsInGroup: " + shape3.IsInGroup);

            // Сохранить результат
            workbook.Save("ShapePropertyIsInGroupDemo2.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


