---
title: "GradientFill.GradientStops"
second_title: "Справочник API Aspose.Cells для .NET"
description: "GradientFill property. Представляет коллекцию точек градиента"
type: docs
url: /ru/net/aspose.cells.drawing/gradientfill/gradientstops/
---
## GradientFill.GradientStops property

Представляет коллекцию градиентных остановок.

```csharp
public GradientStopCollection GradientStops { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyGradientStopsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;
            
            // Добавить прямоугольную фигуру
            Shape shape = shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Установить градиентную заливку
            shape.Fill.FillType = FillType.Gradient;
            GradientFill gradientFill = shape.Fill.GradientFill;
            
            // Очистить любые существующие точки градиента
            gradientFill.GradientStops.Clear();

            // Добавить пользовательские точки градиента
            gradientFill.GradientStops.Add(0.0, Color.Red, 255);
            gradientFill.GradientStops.Add(0.5, Color.Yellow, 255);
            gradientFill.GradientStops.Add(1.0, Color.Green, 255);

            // Продемонстрировать доступ к точкам градиента
            Console.WriteLine("Gradient Stops Count: " + gradientFill.GradientStops.Count);
            Console.WriteLine("First Stop Position: " + gradientFill.GradientStops[0].Position);
            Console.WriteLine("Second Stop Color: " + gradientFill.GradientStops[1].CellsColor);

            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### См. также

* class [GradientStopCollection](../../gradientstopcollection/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


