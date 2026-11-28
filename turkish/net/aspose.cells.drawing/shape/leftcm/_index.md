---
title: "Shape.LeftCM"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin sol sütunundan yatay ofsetini santimetre biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/leftcm/
---
## Shape.LeftCM property

Şeklin sol sütunundan yatay ofsetini santimetre biriminde temsil eder.

```csharp
public double LeftCM { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftCMDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // LeftCM özelliğini ayarla ve al
            shape.LeftCM = 3.0;
            Console.WriteLine("Shape left position (cm): " + shape.LeftCM);

            // Sol konumu 3 cm ise değiştir
            if (shape.LeftCM == 3.0)
            {
                shape.LeftCM = 1.0;
                Console.WriteLine("Adjusted shape left position (cm): " + shape.LeftCM);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


