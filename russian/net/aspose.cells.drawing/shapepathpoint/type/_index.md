---
title: "ShapePathPoint.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapePathPoint. Указывает тип значения текущего объекта"
type: docs
url: /ru/net/aspose.cells.drawing/shapepathpoint/type/
---
## ShapePathPoint.Type property

Указывает тип значения текущего объекта.

```csharp
public ShapePathPointValueType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyTypeDemo
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

                // Добавить точку координаты позиции
                int positionPointIndex = pathPoints.Add(100, 50);
                ShapePathPoint positionPoint = pathPoints[positionPointIndex];

                // Отобразить значение свойства Type для координаты позиции
                Console.WriteLine($"Position Point Type: {positionPoint.Type}");
                Console.WriteLine($"Position Point Type is Position: {positionPoint.Type == ShapePathPointValueType.Position}");

                // Добавить точку маркера угла
                int anglePointIndex = pathPoints.Add(0, 0);
                ShapePathPoint anglePoint = pathPoints[anglePointIndex];
                anglePoint.XAngle = 45;
                anglePoint.YAngle = 90;

                // Отобразить значение свойства Type для маркера угла
                Console.WriteLine($"Angle Point Type: {anglePoint.Type}");
                Console.WriteLine($"Angle Point Type is Angle: {anglePoint.Type == ShapePathPointValueType.Angle}");

                // Создать путь фигуры и добавить точки
                ShapePath path = new ShapePath();
                path.MoveTo(positionPoint.XPixel, positionPoint.YPixel);
                path.ArcTo(anglePoint.XAngle, anglePoint.YAngle, 100, 100);
                path.Close();

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
                workbook.Save("ShapePathPointTypeDemo.xlsx");
                Console.WriteLine("Type property demonstration completed successfully.");
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

* enum [ShapePathPointValueType](../../shapepathpointvaluetype/)
* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


