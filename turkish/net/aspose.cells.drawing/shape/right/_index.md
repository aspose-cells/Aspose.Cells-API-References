---
title: "Shape.Right"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin alt sağ köşe sütunundan piksel biriminde yatay ofsetinin genişliğini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/right/
---
## Shape.Right property

Şeklin alt sağ köşe sütunundan yatay ofsetinin genişliğini, piksel biriminde temsil eder.

```csharp
public int Right { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRightDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Right özelliğini ayarlayın ve alın
            shape.Right = 200;
            Console.WriteLine("Shape Right position: " + shape.Right);

            // Right özelliğini koşullu olarak değiştirin
            if (shape.Right == 200)
                shape.Right = 150;

            Console.WriteLine("Modified Shape Right position: " + shape.Right);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


