---
title: "Shape.X"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape property. Şeklin çalışma sayfası sol kenarından piksel biriminde yatay offsetini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/x/
---
## Shape.X property

Şeklin çalışma sayfasının sol kenarından yatay offsetini alır ve ayarlar, piksel biriminde.

```csharp
public int X { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyXDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // İlk X konumunu ayarla
            shape.X = 200;
            Console.WriteLine("Initial X position: " + shape.X);

            // X konumu 3'e eşitse değiştir (test durumu mantığını göstererek)
            if (shape.X == 3)
            {
                shape.X = 1;
            }
            else
            {
                // Demonstrasyon amacıyla X konumunu 300'e değiştir
                shape.X = 300;
            }

            Console.WriteLine("Final X position: " + shape.X);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


