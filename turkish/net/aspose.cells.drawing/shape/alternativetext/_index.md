---
title: "Shape.AlternativeText"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Shape nesnesinin açıklayıcı alternatif metin dizesini döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/alternativetext/
---
## Shape.AlternativeText property

[`Shape`](../) nesnesinin açıklayıcı (alternatif) metin dizesini döndürür veya ayarlar.

```csharp
public string AlternativeText { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAlternativeTextDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Şekil için alternatif metin ayarla
            shape.AlternativeText = "A rectangle shape with width 100 and height 200";

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeAlternativeTextDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


