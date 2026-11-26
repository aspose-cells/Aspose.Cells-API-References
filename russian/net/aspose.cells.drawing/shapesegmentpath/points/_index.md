---
title: "ShapeSegmentPath.Points"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapeSegmentPath. Возвращает точки в сегменте пути"
type: docs
url: /ru/net/aspose.cells.drawing/shapesegmentpath/points/
---
## ShapeSegmentPath.Points property

Получает точки в сегменте пути

```csharp
public ShapePathPointCollection Points { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathPropertyPointsDemo
    {
        public static void Run()
        {// Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ShapePath path = new ShapePath();

            // Начать новый путь
            path.MoveTo(10, 10);

            // Нарисовать линейный сегмент
            path.LineTo(100, 100);

            // Получить доступ к свойству PathSegementList
            ShapeSegmentPathCollection segmentPaths = path.PathSegementList;

            // Получить доступ к первому пути сегмента
            ShapeSegmentPath segmentPath = segmentPaths[1];

            // Отобразить информацию о точках
            Console.WriteLine("Number of points in segment: " + segmentPath.Points.Count);
            Console.WriteLine("Point coordinates:");
            foreach (ShapePathPoint point in segmentPath.Points)
            {
                Console.WriteLine($"X: {point.X}, Y: {point.Y}");
            }          

            //добавить свободную форму
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

            // Сохраните книгу
            workbook.Save("ShapeSegmentPathPointsDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapePathPointCollection](../../shapepathpointcollection/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


