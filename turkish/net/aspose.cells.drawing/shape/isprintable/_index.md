---
title: "Shape.IsPrintable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Nesnenin yazdırılabilir olup olmadığını gösterir. False ise bu şekil yazdırma sırasında basılmaz"
type: docs
url: /tr/net/aspose.cells.drawing/shape/isprintable/
---
## Shape.IsPrintable property

Nesnenin yazdırılabilir olup olmadığını gösterir. False ise, bu şekil yazdırma sırasında basılmaz.

```csharp
public bool IsPrintable { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsPrintableDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // IsPrintable özelliğini gösterin
            Console.WriteLine("Shape is printable initially: " + shape.IsPrintable);

            // IsPrintable özelliğini değiştirin
            shape.IsPrintable = !shape.IsPrintable;
            Console.WriteLine("Shape is printable after toggle: " + shape.IsPrintable);

            // IsPrintable'ı açıkça false olarak ayarlayın
            shape.IsPrintable = false;
            Console.WriteLine("Shape is printable after setting to false: " + shape.IsPrintable);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


