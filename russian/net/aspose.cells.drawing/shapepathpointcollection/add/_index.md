---
title: "ShapePathPointCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapePathPointCollection. Добавляет точку пути в единицах EMU"
type: docs
url: /ru/net/aspose.cells.drawing/shapepathpointcollection/add/
---
## ShapePathPointCollection.Add method

Добавляет точку пути в единицах EMU.

```csharp
[Obsolete("Use the MoveTo,LineTo,CubicBezierTo and ArcTo methods in ShapePath instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(int x, int y)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| x | Int32 | Координата x. |
| y | Int32 | Координата y. |

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте методы MoveTo,LineTo,CubicBezierTo и ArcTo в ShapePath. Этот метод будет удалён через 12 месяцев, начиная с августа 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте коллекцию точек пути формы
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();

            try
            {
                // Вызовите метод Add с параметрами (Int32, Int32)
                pathPoints.Add(50, 10);
                pathPoints.Add(50, 50);
                pathPoints.Add(10, 50);

                // Создать путь фигуры и добавить точки
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

                // Сохранить результат
                workbook.Save("ShapePathPointCollectionMethodAddWithInt32Int32Demo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ShapePathPointCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


