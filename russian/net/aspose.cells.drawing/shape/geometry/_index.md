---
title: "Shape.Geometry"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает геометрию"
type: docs
url: /ru/net/aspose.cells.drawing/shape/geometry/
---
## Shape.Geometry property

Получает геометрию

```csharp
public Geometry Geometry { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyGeometryDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму с правильными параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Проверьте свойства геометрии
            if (shape.Geometry != null)
            {
                Console.WriteLine("Shape has geometry path with " + shape.Geometry.ShapeAdjustValues.Count + " adjustment points");
                
                // Добавьте точку регулировки (демонстрируя изменение геометрии)
                shape.Geometry.ShapeAdjustValues.Add("adj1", 0.5);
                Console.WriteLine("Added adjustment point. Total now: " + shape.Geometry.ShapeAdjustValues.Count);
            }

            // Сохраните книгу
            workbook.Save("ShapeGeometryDemo.xlsx");
        }
    }
}
```

### См. также

* class [Geometry](../../geometry/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


