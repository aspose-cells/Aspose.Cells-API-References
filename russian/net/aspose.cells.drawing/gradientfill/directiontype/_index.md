---
title: "GradientFill.DirectionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GradientFill. Возвращает тип направления градиента"
type: docs
url: /ru/net/aspose.cells.drawing/gradientfill/directiontype/
---
## GradientFill.DirectionType property

Получает тип направления градиента.

```csharp
public GradientDirectionType DirectionType { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyDirectionTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму для демонстрации градиентной заливки
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 5);

            // Установить свойства градиентной заливки
            FillFormat fillFormat = shape.Fill;
            fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.DiagonalDown, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Вывести тип направления градиента
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Сохраните книгу
            workbook.Save("GradientDirectionTypeExample.xlsx");
        }
    }
}
```

### См. также

* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


