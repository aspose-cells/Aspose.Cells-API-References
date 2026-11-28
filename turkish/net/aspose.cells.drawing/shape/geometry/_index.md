---
title: "Shape.Geometry"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Şekil özelliği. Geometrisini alır"
type: docs
url: /tr/net/aspose.cells.drawing/shape/geometry/
---
## Shape.Geometry property

Geometriyi alır

```csharp
public Geometry Geometry { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyGeometryDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Geometri özelliklerini kontrol edin
            if (shape.Geometry != null)
            {
                Console.WriteLine("Shape has geometry path with " + shape.Geometry.ShapeAdjustValues.Count + " adjustment points");
                
                // Bir ayarlama noktası ekleyin (geometri değişikliğini göstererek)
                shape.Geometry.ShapeAdjustValues.Add("adj1", 0.5);
                Console.WriteLine("Added adjustment point. Total now: " + shape.Geometry.ShapeAdjustValues.Count);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeGeometryDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Geometry](../../geometry/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


