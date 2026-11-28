---
title: "Shape.GetConnectionPoints"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape yöntemi. Bağlantı noktalarını alır"
type: docs
url: /tr/net/aspose.cells.drawing/shape/getconnectionpoints/
---
## Shape.GetConnectionPoints method

Bağlantı noktalarını al

```csharp
public float[][] GetConnectionPoints()
```

### Dönüş Değeri

[X,Y] pairs of the connection point. Every item is a float[2] array, [0] represents x and [1] represents y.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetConnectionPointsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Şeklin bağlantı noktalarını alın
            float[][] points = shape.GetConnectionPoints();

            // Bağlantı noktalarını çıktı olarak verin
            Console.WriteLine("Connection Points:");
            for (int i = 0; i < points.Length; i++)
            {
                Console.WriteLine($"Point {i + 1}: X={points[i][0]}, Y={points[i][1]}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


