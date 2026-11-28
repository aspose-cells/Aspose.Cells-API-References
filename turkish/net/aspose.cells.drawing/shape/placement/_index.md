---
title: "Shape.Placement"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Çizim nesnesinin altındaki hücrelere nasıl bağlandığını temsil eder. Bu özellik, bir nesnenin çalışma sayfasındaki konumunu kontrol eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/placement/
---
## Shape.Placement property

Çizim nesnesinin altındaki hücrelere nasıl bağlandığını temsil eder. Özellik, bir nesnenin çalışma sayfasındaki konumunu kontrol eder.

```csharp
public PlacementType Placement { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyPlacementDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 50);

            // Placement özelliğini göster
            Console.WriteLine("Original Placement: " + shape.Placement);
            
            // Yerleşim tipini değiştirin
            shape.Placement = PlacementType.MoveAndSize;
            Console.WriteLine("Modified Placement: " + shape.Placement);

            // Çalışma kitabını kaydedin
            workbook.Save("ShapePlacementDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PlacementType](../../placementtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


