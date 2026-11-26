---
title: "GradientStop.CellsColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GradientStop. Получает цвет этой градиентной остановки"
type: docs
url: /ru/net/aspose.cells.drawing/gradientstop/cellscolor/
---
## GradientStop.CellsColor property

Получает цвет этой градиентной остановки.

```csharp
public CellsColor CellsColor { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopPropertyCellsColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавить фигуру с градиентной заливкой
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
                shape.Fill.FillType = FillType.Gradient;
                GradientFill gradientFill = shape.Fill.GradientFill;
                gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);

                // Создать цвет для градиентной точки
                CellsColor color = workbook.CreateCellsColor();
                color.Color = Color.Blue;

                // Добавить градиентную точку
                gradientFill.GradientStops.Add(0, color, 30);

                // Получите доступ к градиентной остановке и отобразите её свойства CellsColor
                GradientStop stop = gradientFill.GradientStops[0];
                CellsColor stopColor = stop.CellsColor;

                Console.WriteLine("Gradient Stop CellsColor Properties:");
                Console.WriteLine("Color Type: " + stopColor.Type);
                Console.WriteLine("RGB Color: " + stopColor.Color);
                Console.WriteLine("ARGB Value: " + stopColor.Argb);
                Console.WriteLine("Transparency: " + stopColor.Transparency);

                // Сохраните книгу
                workbook.Save("GradientStopCellsColorDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


