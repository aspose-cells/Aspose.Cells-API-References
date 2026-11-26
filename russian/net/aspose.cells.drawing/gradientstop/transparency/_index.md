---
title: "GradientStop.Transparency"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GradientStop. Возвращает или задает степень прозрачности области значением от 0.0 непрозрачный до 1.0 прозрачный"
type: docs
url: /ru/net/aspose.cells.drawing/gradientstop/transparency/
---
## GradientStop.Transparency property

Возвращает или задает степень прозрачности области значением от 0.0 (непрозрачный) до 1.0 (прозрачный).

```csharp
public double Transparency { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить фигуру с градиентной заливкой
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
            shape.Fill.FillType = FillType.Gradient;
            GradientFill gradientFill = shape.Fill.GradientFill;
            gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);

            // Создать цвет для градиентной точки
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Blue;

            // Добавьте градиентную остановку с начальной прозрачностью
            gradientFill.GradientStops.Add(0, color, 30);

            // Получить доступ к градиентной точке
            GradientStop stop = gradientFill.GradientStops[0];

            // Отобразите и измените прозрачность
            Console.WriteLine("Initial Transparency: " + stop.Transparency);
            stop.Transparency = 0.7;
            Console.WriteLine("Modified Transparency: " + stop.Transparency);

            // Добавьте еще одну остановку для визуального сравнения
            CellsColor color2 = workbook.CreateCellsColor();
            color2.Color = Color.Green;
            gradientFill.GradientStops.Add(1, color2, 30);

            // Сохраните книгу
            workbook.Save("GradientStopTransparencyDemo.xlsx");
        }
    }
}
```

### См. также

* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


