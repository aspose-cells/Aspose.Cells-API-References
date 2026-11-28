---
title: "Shape.Title"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Mevcut şekil nesnesinin başlık açıklamasını belirtir"
type: docs
url: /tr/net/aspose.cells.drawing/shape/title/
---
## Shape.Title property

Mevcut şekil nesnesinin başlığını (alt yazısını) belirtir.

```csharp
public string Title { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTitleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Şeklin başlığını ayarla
            shape.Title = "title1";

            // Başlığın ayarlandığını doğrula
            Console.WriteLine("Shape title: " + shape.Title);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


