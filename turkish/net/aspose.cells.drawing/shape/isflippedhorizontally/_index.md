---
title: "Shape.IsFlippedHorizontally"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin yatay olarak çevrilip çevrilmediğini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/isflippedhorizontally/
---
## Shape.IsFlippedHorizontally property

Şeklin yatay olarak çevrilip çevrilmediğini alır ve ayarlar.

```csharp
public bool IsFlippedHorizontally { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsFlippedHorizontallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir örnek şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Henüz çevrilmemişse kontrol et ve yatay olarak çevir
            if (shape.IsFlippedHorizontally == false)
            {
                shape.IsFlippedHorizontally = true;
                Console.WriteLine("Shape was flipped horizontally");
            }
            else
            {
                Console.WriteLine("Shape was already flipped horizontally");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


