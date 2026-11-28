---
title: "Shape.IsTextWrapped"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Metin içeren şeklin metin sarma tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/istextwrapped/
---
## Shape.IsTextWrapped property

Metin içeren şeklin metin sarma tipini alır ve ayarlar.

```csharp
public bool IsTextWrapped { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir şekil ekleyin ve bazı metinler ayarlayın
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            shape.Text = "This is a sample text that will demonstrate text wrapping functionality";

            // IsTextWrapped özelliğini göster
            Console.WriteLine("Initial IsTextWrapped value: " + shape.IsTextWrapped);
            
            // Metin sarma özelliğini değiştirin
            shape.IsTextWrapped = !shape.IsTextWrapped;
            Console.WriteLine("After toggle, IsTextWrapped value: " + shape.IsTextWrapped);

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeTextWrappingDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


