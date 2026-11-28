---
title: "Shape.TextVerticalAlignment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin metin dikey hizalama türünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/textverticalalignment/
---
## Shape.TextVerticalAlignment property

Şeklin metin dikey hizalama türünü alır ve ayarlar.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Metni ve hizalamayı ayarla
            shape.Text = "Vertical Alignment Demo";
            shape.TextVerticalAlignment = TextAlignmentType.Bottom;
            
            Console.WriteLine("Initial Vertical Alignment: " + shape.TextVerticalAlignment);

            // Dikey hizalamayı değiştir
            if (shape.TextVerticalAlignment == TextAlignmentType.Bottom)
            {
                shape.TextVerticalAlignment = TextAlignmentType.Center;
            }

            Console.WriteLine("Updated Vertical Alignment: " + shape.TextVerticalAlignment);

            // Çalışma kitabını kaydedin
            workbook.Save("TextVerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


