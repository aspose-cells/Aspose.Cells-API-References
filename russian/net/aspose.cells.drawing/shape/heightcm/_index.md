---
title: "Shape.HeightCM"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет высоту фигуры в сантиметрах"
type: docs
url: /ru/net/aspose.cells.drawing/shape/heightcm/
---
## Shape.HeightCM property

Представляет высоту фигуры в сантиметрах.

```csharp
public double HeightCM { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Установить высоту в сантиметрах
            shape.HeightCM = 3;
            Console.WriteLine("Shape height: " + shape.HeightCM + " cm");

            // Изменить высоту, если она 3 см
            if (shape.HeightCM == 3)
            {
                shape.HeightCM = 1;
                Console.WriteLine("Modified shape height: " + shape.HeightCM + " cm");
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


