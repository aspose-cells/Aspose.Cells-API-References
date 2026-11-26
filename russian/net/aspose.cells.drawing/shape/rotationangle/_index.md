---
title: "Shape.RotationAngle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задаёт вращение формы"
type: docs
url: /ru/net/aspose.cells.drawing/shape/rotationangle/
---
## Shape.RotationAngle property

Получает и задает вращение фигуры.

```csharp
public double RotationAngle { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 100, 200, 0, 0);

            // Установить угол поворота на 60 градусов
            shape.RotationAngle = 60;
            Console.WriteLine("Shape rotation angle set to: " + shape.RotationAngle);

            // Получить текущий угол поворота
            double currentAngle = shape.RotationAngle;
            Console.WriteLine("Current shape rotation angle: " + currentAngle);

            // Сохраните книгу
            workbook.Save("ShapeRotationDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


