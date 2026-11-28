---
title: "Shape.IsHidden"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Şekil özelliği. Nesnenin görünür olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/shape/ishidden/
---
## Shape.IsHidden property

Nesnenin görünür olup olmadığını gösterir.

```csharp
public bool IsHidden { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // IsHidden özelliğini false (görünür) olarak ayarla
            shape.IsHidden = false;
            Console.WriteLine("Shape is visible: " + !shape.IsHidden);

            // IsHidden özelliğini true (gizli) olarak ayarla
            shape.IsHidden = true;
            Console.WriteLine("Shape is hidden: " + shape.IsHidden);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


