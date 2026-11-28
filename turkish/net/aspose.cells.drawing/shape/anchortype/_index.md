---
title: "Shape.AnchorType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şekil ankraj yer tutucusunun türünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/anchortype/
---
## Shape.AnchorType property

Şekil çapa yer tutucusunun tipini alır ve ayarlar.

```csharp
public ShapeAnchorType AnchorType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAnchorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Varsayılan ankraj türüyle bir şekil ekleyin
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
            
            // Ankraj türünü kontrol edin ve değiştirin
            if (shape.AnchorType == ShapeAnchorType.OneCellAnchor)
            {
                shape.AnchorType = ShapeAnchorType.TwoCellAnchor;
                Console.WriteLine("Anchor type changed to TwoCellAnchor");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("ShapeAnchorTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ShapeAnchorType](../../shapeanchortype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


