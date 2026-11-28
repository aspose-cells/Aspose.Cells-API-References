---
title: "Shape.WidthScale"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Orijinal resim genişliğinin yüzde birimi olarak genişlik ölçeğini alır ve ayarlar. Şekil resim değilse WidthScale özelliği yalnızca 100 döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/shape/widthscale/
---
## Shape.WidthScale property

Orijinal resim genişliğinin yüzde biriminde genişlik ölçeğini alır ve ayarlar. Şekil resim değilse, WidthScale özelliği yalnızca 100 döndürür;

```csharp
public int WidthScale { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthScaleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // İlk genişlik ölçeğini ayarla
            shape.WidthScale = 50;
            Console.WriteLine("Initial WidthScale: " + shape.WidthScale);

            // Koşul karşılandığında genişlik ölçeğini değiştir
            if (shape.WidthScale == 50)
            {
                shape.WidthScale = 75;
                Console.WriteLine("Updated WidthScale: " + shape.WidthScale);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeWidthScaleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


