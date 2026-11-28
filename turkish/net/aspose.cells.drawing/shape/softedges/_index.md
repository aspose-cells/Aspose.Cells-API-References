---
title: "Shape.SoftEdges"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Şekil özelliği. Kenarlara uygulanacak bulanıklık yarıçapını nokta biriminde alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/softedges/
---
## Shape.SoftEdges property

Kenarlar için uygulanacak bulanıklık yarıçapını puan (point) biriminde alır ve ayarlar.

```csharp
public double SoftEdges { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySoftEdgesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // 5 nokta yarıçaplı (0.5d = 5 nokta) yumuşak kenar etkisini ayarla
            shape.SoftEdges = 0.5d;

            // Çalışma kitabını kaydedin
            workbook.Save("SoftEdgesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


