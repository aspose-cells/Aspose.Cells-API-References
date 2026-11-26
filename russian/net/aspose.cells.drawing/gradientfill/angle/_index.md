---
title: "GradientFill.Angle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GradientFill. Угол линейного заполнения"
type: docs
url: /ru/net/aspose.cells.drawing/gradientfill/angle/
---
## GradientFill.Angle property

Угол линейной заливки.

```csharp
public float Angle { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyAngleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму, чтобы продемонстрировать заливку градиентом
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // Установить свойства градиентной заливки
            shape.Fill.FillType = FillType.Gradient;
            shape.Fill.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromCenter);
            shape.Fill.GradientFill.Angle = 45; // Set the angle to 45 degrees

            // Установить цвета градиента
            shape.Fill.GradientFill.SetTwoColorGradient(
                Color.Red, 
                Color.Blue, 
                GradientStyleType.Horizontal, 
                1);

            // Сохраните книгу
            workbook.Save("GradientFillAngleDemo.xlsx");

            Console.WriteLine("Demo completed. File saved with gradient fill at 45 degree angle.");
        }
    }
}
```

### См. также

* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


