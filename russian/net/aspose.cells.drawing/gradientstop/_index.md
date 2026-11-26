---
title: "Класс GradientStop"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.GradientStop класс. Представляет градиентную остановку"
type: docs
url: /ru/net/aspose.cells.drawing/gradientstop/
---
## GradientStop class

Представляет градиентную остановку.

```csharp
public class GradientStop
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/gradientstop/cellscolor/) { get; } | Получает цвет этой градиентной остановки. |
| [Position](../../aspose.cells.drawing/gradientstop/position/) { get; set; } | Позиция остановки. |
| [Transparency](../../aspose.cells.drawing/gradientstop/transparency/) { get; set; } | Возвращает или задает степень прозрачности области значением от 0.0 (непрозрачный) до 1.0 (прозрачный). |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassGradientStopDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
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

                // Получить доступ к градиентной точке
                GradientStop stop = gradientFill.GradientStops[0];

                // Продемонстрируйте базовую функциональность
                Console.WriteLine("GradientStop instance created successfully");
                Console.WriteLine("Position: " + stop.Position);
                Console.WriteLine("Transparency: " + stop.Transparency);
                Console.WriteLine("CellsColor Type: " + stop.CellsColor.Type);

                // Изменить свойства
                stop.Position = 0.5;
                stop.Transparency = 0.7;

                Console.WriteLine("Modified Position: " + stop.Position);
                Console.WriteLine("Modified Transparency: " + stop.Transparency);

                // Сохраните книгу
                workbook.Save("GradientStopDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientStop: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


