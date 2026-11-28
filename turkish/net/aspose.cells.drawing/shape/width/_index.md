---
title: "Shape.Width"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin piksel birimindeki genişliğini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/width/
---
## Shape.Width property

Şeklin genişliğini, piksel biriminde temsil eder.

```csharp
public int Width { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 50);

            // İlk genişliği ayarla ve göster
            shape.Width = 300;
            Console.WriteLine("Initial width: " + shape.Width);

            // Koşula göre genişliği değiştir
            if (shape.Width == 300)
                shape.Width = 150;

            Console.WriteLine("Modified width: " + shape.Width);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


