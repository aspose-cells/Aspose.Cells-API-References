---
title: "Shape.Y"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin çalışma sayfası üst kenarından piksel cinsinden dikey offsetini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/y/
---
## Shape.Y property

Şeklin çalışma sayfası üst kenarından piksel biriminde dikey ofsetini alır ve ayarlar.

```csharp
public int Y { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyYDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Y özelliğini ayarla ve göster
            shape.Y = 200;
            Console.WriteLine("Shape Y position: " + shape.Y);

            // Koşula göre Y konumunu değiştir
            if (shape.Y == 200)
                shape.Y = 100;

            Console.WriteLine("Updated Shape Y position: " + shape.Y);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


