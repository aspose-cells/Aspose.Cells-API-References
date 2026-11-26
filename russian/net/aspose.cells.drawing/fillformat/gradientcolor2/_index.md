---
title: "FillFormat.GradientColor2"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FillFormat. Возвращает второй градиентный цвет для указанного заполнения"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/gradientcolor2/
---
## FillFormat.GradientColor2 property

Возвращает градиентный цвет 2 для указанной заливки.

```csharp
public Color GradientColor2 { get; }
```

### Примечания

Только когда тип градиентного цвета равен GradientColorType.TwoColors, это свойство имеет смысл.

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientColor2Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте прямоугольную форму с двухцветным градиентным заполнением
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 200);
            FillFormat fill = rectangle.Fill;
            
            fill.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 2);

            // Проверьте свойства градиентных цветов
            Console.WriteLine("GradientColor2: " + fill.GradientColor2);
        }
    }
}
```

### См. также

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


