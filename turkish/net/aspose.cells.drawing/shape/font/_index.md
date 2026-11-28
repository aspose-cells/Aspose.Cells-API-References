---
title: "Shape.Font"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin yazı tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/font/
---
## Shape.Font property

Şeklin yazı tipini temsil eder.

```csharp
public Font Font { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFontDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Şeklin yazı tipi özelliklerine eriş ve değiştir
            Aspose.Cells.Font font = shape.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.Color = Color.Red;

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeFontDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../../../aspose.cells/font/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


