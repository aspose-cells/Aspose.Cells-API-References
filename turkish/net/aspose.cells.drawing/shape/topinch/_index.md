---
title: "Shape.TopInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin üst satırından inç cinsinden dikey offsetini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/topinch/
---
## Shape.TopInch property

Şeklin üst satırından dikey ofsetini inç biriminde temsil eder.

```csharp
public double TopInch { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopInchDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // TopInch özelliğini ayarla ve göster
            shape.TopInch = 3;
            Console.WriteLine("Shape Top position (inches): " + shape.TopInch);

            // TopInch 3 ise değiştir
            if (shape.TopInch == 3)
            {
                shape.TopInch = 1;
                Console.WriteLine("Modified Shape Top position (inches): " + shape.TopInch);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeTopInchDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


