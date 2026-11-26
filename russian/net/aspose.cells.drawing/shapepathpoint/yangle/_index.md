---
title: "ShapePathPoint.YAngle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapePathPoint. Когда объект является маркером угла, получайте или задавайте второй угол в градусах"
type: docs
url: /ru/net/aspose.cells.drawing/shapepathpoint/yangle/
---
## ShapePathPoint.YAngle property

Когда объект является маркером угла, получайте или задавайте второй угол в градусах.

```csharp
public int YAngle { get; set; }
```

### Примечания

Если этот угол является углом разворота дуги. Этот угол указывает, насколько далеко по углу вдоль предполагаемого пути круга будет продолжена дуга. Продление от начального угла всегда будет происходить по часовой стрелке вокруг предполагаемого круга.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYAngleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создайте коллекцию точек пути формы
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // Добавьте точки с маркерами углов (используя XAngle и YAngle)
                ShapePathPoint point1 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point1.XAngle = 45;  // First angle in degrees
                point1.YAngle = 90;  // Second angle in degrees

                // Отобразите значение YAngle
                Console.WriteLine($"Point 1 YAngle: {point1.YAngle} degrees");

                // Создать другую точку с разными углами
                ShapePathPoint point2 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point2.XAngle = 30;
                point2.YAngle = 60;

                // Отобразите значение YAngle
                Console.WriteLine($"Point 2 YAngle: {point2.YAngle} degrees");

                // Создать путь фигуры и добавить дугу, используя маркеры углов
                ShapePath path = new ShapePath();
                path.ArcTo(point1.XAngle, point1.YAngle, 100, 100);

                // Добавить свободноформенную фигуру в лист
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // Сохраните книгу
                workbook.Save("YAngleDemo.xlsx");
                Console.WriteLine("YAngle property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


