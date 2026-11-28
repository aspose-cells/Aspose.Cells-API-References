---
title: "Shape.Top"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin üst satırından piksel biriminde dikey kaymasını temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/top/
---
## Shape.Top property

Şeklin üst satırından dikey ofsetini piksel biriminde temsil eder.

```csharp
public int Top { get; set; }
```

### Açıklamalar

Şekil grafik içinde ise, şeklin üst kenarından dikey offsetini temsil eder.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // İlk üst konumu ayarlayın
            shape.Top = 50;
            Console.WriteLine("Initial Top position: " + shape.Top);

            // Üst konumu 3'e eşitse değiştirin (test durumu mantığını göstererek)
            if (shape.Top == 3)
            {
                shape.Top = 1;
            }
            else
            {
                // Demonstrasyon için 3 olarak ayarlayın ve ardından test durumu mantığını uygulayın
                shape.Top = 3;
                if (shape.Top == 3)
                {
                    shape.Top = 1;
                    Console.WriteLine("Modified Top position: " + shape.Top);
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


