---
title: "Класс ShapeGuide"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.ShapeGuide. Инкапсулирует направляющую фигуры, указывающую наличие направляющей, которая будет использоваться для управления геометрией указанной фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shapeguide/
---
## ShapeGuide class

Инкапсулирует руководство по фигурам, указывающее наличие руководства по фигурам, которое будет использоваться для управления геометрией указанной фигуры.

```csharp
public class ShapeGuide : BaseShapeGuide
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Value](../../aspose.cells.drawing/shapeguide/value/) { get; set; } | Получает или задает значение этой направляющей |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeGuideDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 0, 0, 100, 100, 100, 100);
                
                // Создайте и добавьте направляющую фигуры с необходимыми параметрами
                int guideIndex = shape.Geometry.ShapeAdjustValues.Add("Guide1", 0.2);
                ShapeGuide guide = shape.Geometry.ShapeAdjustValues[guideIndex];
                
                Console.WriteLine($"ShapeGuide created with Value: {guide.Value}");
                
                workbook.Save("DrawingClassShapeGuideDemo.xlsx");
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

* class [BaseShapeGuide](../baseshapeguide/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


