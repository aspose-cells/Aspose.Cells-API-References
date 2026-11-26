---
title: "Класс Geometry"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.Geometry. Представляет геометрическую фигуру"
type: docs
url: /ru/net/aspose.cells.drawing/geometry/
---
## Geometry class

Представляет геометрическую форму.

```csharp
public abstract class Geometry
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | Получает коллекцию значений регулировки фигуры |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    
    public class DrawingClassGeometryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру на лист
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Получить доступ к геометрии фигуры
            Geometry geometry = rectangle.Geometry;

            // Добавить направляющие регулировки фигуры непосредственно в коллекцию
            geometry.ShapeAdjustValues.Add("Roundness", 0.3);
            geometry.ShapeAdjustValues.Add("Angle", 45.0);

            // Сохранить изменённую книгу
            workbook.Save("GeometryDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


