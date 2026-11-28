---
title: "Shape.UpperLeftRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Üst satır indeksini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/upperleftrow/
---
## Shape.UpperLeftRow property

Üst satır indeksini temsil eder.

```csharp
public int UpperLeftRow { get; set; }
```

### Açıklamalar

Şekil bir şekil içinde veya bir grup içinde ise, UpperLeftRow yoksayılacaktır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperLeftRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // UpperLeftRow özelliğini ayarlayın ve gösterin
            shape.UpperLeftRow = 3;
            Console.WriteLine("Shape's initial topRow: " + shape.UpperLeftRow);

            // Koşula göre UpperLeftRow değerini değiştirin
            if (shape.UpperLeftRow == 3)
                shape.UpperLeftRow = 1;

            Console.WriteLine("Shape's modified topRow: " + shape.UpperLeftRow);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


