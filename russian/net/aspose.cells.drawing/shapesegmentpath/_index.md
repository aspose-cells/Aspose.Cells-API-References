---
title: "Класс ShapeSegmentPath"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.ShapeSegmentPath. Представляет сегмент пути в пути свободной формы"
type: docs
url: /ru/net/aspose.cells.drawing/shapesegmentpath/
---
## ShapeSegmentPath class

Представляет сегмент пути в пути произвольной формы.

```csharp
public class ShapeSegmentPath
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Points](../../aspose.cells.drawing/shapesegmentpath/points/) { get; } | Получает точки в сегменте пути |
| [Type](../../aspose.cells.drawing/shapesegmentpath/type/) { get; } | Получает тип сегмента пути |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeSegmentPathDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить свободную форму на лист
            Shape shape = worksheet.Shapes.AddFreeform(0, 0, 0, 0, 200, 200, new ShapePath[] { new ShapePath() });

            // Получить геометрический путь фигуры
            CustomGeometry geometry = shape.Geometry as CustomGeometry;
            ShapePath shapePath = geometry.Paths[0];

            // Получить доступ к первому сегменту пути (если существует)
            if (shapePath.PathSegementList.Count > 0)
            {
                ShapeSegmentPath segmentPath = shapePath.PathSegementList[0];

                // Продемонстрировать свойства ShapeSegmentPath
                Console.WriteLine("Segment Path Type: " + segmentPath.Type);
                Console.WriteLine("Number of Points: " + segmentPath.Points.Count);

                // Итерировать точки в сегменте пути
                foreach (ShapePathPoint point in segmentPath.Points)
                {
                    Console.WriteLine($"Point coordinates: X={point.X}, Y={point.Y}");
                }
            }

            // Сохраните книгу
            workbook.Save("ShapeSegmentPathDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


