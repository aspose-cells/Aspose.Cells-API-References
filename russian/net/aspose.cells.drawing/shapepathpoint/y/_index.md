---
title: "ShapePathPoint.Y"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapePathPoint. Возвращает координату y для этой координаты позиции. Единица EMUs"
type: docs
url: /ru/net/aspose.cells.drawing/shapepathpoint/y/
---
## ShapePathPoint.Y property

Возвращает координату y для этой координаты позиции. Единица EMUs.

```csharp
[Obsolete("Use ShapePathPoint.YPixel and ShapePathPoint.YAngle properties instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Y { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойства ShapePathPoint.YPixel и ShapePathPoint.YAngle. Это свойство будет удалено через 12 месяцев, начиная с августа 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте коллекцию точек пути формы и добавьте точки
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(50, 10);
            pathPoints.Add(50, 50);
            pathPoints.Add(10, 50);

            // Получите доступ к точкам с помощью свойства Item
            Console.WriteLine("First point coordinates:");
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"X: {firstPoint.X}, Y: {firstPoint.Y}");

            Console.WriteLine("\nAll points in collection:");
            for (int i = 0; i < pathPoints.Count; i++)
            {
                ShapePathPoint point = pathPoints[i];
                Console.WriteLine($"Point {i}: X={point.X}, Y={point.Y}");
            }

            // Создайте путь формы, используя точки
            ShapePath path = new ShapePath();

            // Перейти к начальной точке
            path.MoveTo(10, 10);

            foreach (ShapePathPoint point in pathPoints)
            {
                path.LineTo(point.X, point.Y);
            }
            path.Close();

            // Добавьте произвольную форму с настроенным путем
            Shape shape = worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path }
                );

            // Сохранить изменённую книгу
            workbook.Save("ShapePathPointYDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


