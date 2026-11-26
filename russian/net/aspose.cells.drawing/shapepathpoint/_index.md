---
title: "Класс ShapePathPoint"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.ShapePathPoint. Указывает координаты позиции или маркеры углов. Координаты позиции представляют координаты пути в пространстве координат, например X/Y. Маркеры углов указывают изменения угла в пути, например начальный и конечный углы дуги."
type: docs
url: /ru/net/aspose.cells.drawing/shapepathpoint/
---
## ShapePathPoint class

Укажите координаты положения или маркеры углов. Координаты положения представляют координаты пути в пространстве координат (например, X/Y). Маркеры углов указывают изменения угла в пути (например, начальный и конечный углы дуги).

```csharp
public class ShapePathPoint
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Type](../../aspose.cells.drawing/shapepathpoint/type/) { get; } | Указывает тип значения текущего объекта. |
| [X](../../aspose.cells.drawing/shapepathpoint/x/) { get; set; } | (**Obsolete.**) Получает и задает координату x для этой координаты позиции. Единица EMU. |
| [XAngle](../../aspose.cells.drawing/shapepathpoint/xangle/) { get; set; } | Когда объект является маркером угла, получайте или задавайте первый угол в градусах. |
| [XPixel](../../aspose.cells.drawing/shapepathpoint/xpixel/) { get; set; } | Когда объект является координатой позиции, получайте или задавайте координату x в пикселях. |
| [Y](../../aspose.cells.drawing/shapepathpoint/y/) { get; set; } | (**Obsolete.**) Получает координату y для этой координаты позиции. Единица EMU. |
| [YAngle](../../aspose.cells.drawing/shapepathpoint/yangle/) { get; set; } | Когда объект является маркером угла, получайте или задавайте второй угол в градусах. |
| [YPixel](../../aspose.cells.drawing/shapepathpoint/ypixel/) { get; set; } | Когда объект является координатой позиции, получайте или задавайте координату y в пикселях. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathPointDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Добавить форму, которая будет содержать точки пути со всеми необходимыми параметрами.
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 10, 10, 200, 200);
                
                // Получить точки геометрического пути.
                CustomGeometry geometry = shape.Geometry as CustomGeometry;
                if (geometry != null && geometry.Paths.Count > 0)
                {
                    ShapePath path = geometry.Paths[0];
                    
                    // Получить доступ к существующей точке пути (если доступна).
                    if (path.PathSegementList.Count > 0)
                    {
                        // Получить первую точку (фактическая реализация может различаться в зависимости от типа сегмента).
                        ShapePathPoint point = path.PathSegementList[0].Points[0];
                        
                        // Отобразить координаты точки
                        Console.WriteLine($"ShapePathPoint at X: {point.X}, Y: {point.Y}");
                    }
                }
                
                // Сохраните книгу
                workbook.Save("ShapePathPointDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathPoint: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


