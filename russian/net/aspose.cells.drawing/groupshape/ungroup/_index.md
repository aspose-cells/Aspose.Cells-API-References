---
title: "GroupShape.Ungroup"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GroupShape. Разгруппирует элементы фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/groupshape/ungroup/
---
## GroupShape.Ungroup method

Разгруппировать элементы фигуры.

```csharp
public void Ungroup()
```

### Примечания

Если групповая фигура сгруппирована другой групповой фигурой, ничего не будет сделано.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GroupShapeMethodUngroupDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить две прямоугольные фигуры
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 50);
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 0, 3, 0, 100, 50);

            // Сгруппировать фигуры в GroupShape
            GroupShape groupShape = worksheet.Shapes.Group(new Shape[] { shape1, shape2 });

            try
            {
                // Выполнить метод Ungroup
                groupShape.Ungroup();
                Console.WriteLine("Shapes ungrouped successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ungrouping: {ex.Message}");
            }

            workbook.Save("GroupShapeUngroupDemo.xlsx");
        }
    }
}
```

### См. также

* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


