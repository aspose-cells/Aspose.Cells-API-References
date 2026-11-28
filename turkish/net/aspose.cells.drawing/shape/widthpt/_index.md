---
title: "Shape.WidthPt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin genişliğini nokta biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/widthpt/
---
## Shape.WidthPt property

Şeklin genişliğini puan biriminde temsil eder.

```csharp
public double WidthPt { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthPtDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Genişliği nokta cinsinden ayarla ve al
            shape.WidthPt = 150;
            Console.WriteLine("Shape width in points: " + shape.WidthPt);

            // Koşul sağlandığında genişliği değiştirin
            if (shape.WidthPt == 150)
            {
                shape.WidthPt = 100;
                Console.WriteLine("Modified shape width in points: " + shape.WidthPt);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


