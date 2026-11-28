---
title: "Shape.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Şekil özelliği. Şeklin adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/name/
---
## Shape.Name property

Şeklin adını alır ve ayarlar.

```csharp
public string Name { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir şekil ekleyin ve adını ayarlayın
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            shape.Name = "shape1";
            
            // Adın ayarlandığını doğrulayın
            Console.WriteLine("Shape name: " + shape.Name);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


