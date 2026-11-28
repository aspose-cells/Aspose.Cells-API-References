---
title: "Shape.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Otomatik şekil tipini alır"
type: docs
url: /tr/net/aspose.cells.drawing/shape/type/
---
## Shape.Type property

Otomatik şekil tipini alır.

```csharp
public AutoShapeType Type { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 100, 150, 0, 0);

            // Şekil tipini al ve göster
            AutoShapeType autoShapeType = shape.Type;
            Console.WriteLine("Shape Type: " + autoShapeType);

            // Şekil tipini değiştiremezsiniz çünkü Type özelliği yalnızca okunur
            // Bunun yerine farklı tipte yeni bir şekil oluşturun
            Shape ovalShape = worksheet.Shapes.AddAutoShape(AutoShapeType.Oval, 1, 1, 100, 150, 0, 0);
            Console.WriteLine("New Shape Type: " + ovalShape.Type);
        }
    }
}
```

### Ayrıca Bakınız

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


