---
title: "Shape.WidthCM"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin genişliğini santimetre biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/widthcm/
---
## Shape.WidthCM property

Şeklin genişliğini santimetre biriminde temsil eder.

```csharp
public double WidthCM { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 100, 100);

            // Genişliği santimetre cinsinden ayarlayın
            shape.WidthCM = 3.5;
            Console.WriteLine("Shape width set to: " + shape.WidthCM + " cm");

            // Koşulu karşılıyorsa genişliği değiştir
            if (shape.WidthCM == 3.5)
            {
                shape.WidthCM = 2.0;
                Console.WriteLine("Shape width changed to: " + shape.WidthCM + " cm");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


