---
title: "Shape.Spt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Şekil özelliği. Bir uygulamanın belirli şekli tanımlı bir şekil türüyle ilişkilendirmek için kullanabileceği isteğe bağlı bir sayı belirtir"
type: docs
url: /tr/net/aspose.cells.drawing/shape/spt/
---
## Shape.Spt property

Bir uygulamanın belirli şekli tanımlı bir şekil türüyle ilişkilendirmek için kullanabileceği isteğe bağlı bir sayıyı belirtir.

```csharp
public int Spt { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySptDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 100, 100, 100, 100);

            // Spt özelliğini al ve görüntüle
            int spt = shape.Spt;
            Console.WriteLine("Shape Spt value: " + spt);

            // Farklı Spt değerini göstermek için yeni bir oval şekil oluşturun
            Shape ovalShape = worksheet.Shapes.AddShape(MsoDrawingType.Oval, 1, 1, 100, 100, 100, 100);
            Console.WriteLine("Oval shape Spt value: " + ovalShape.Spt);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


