---
title: "Shape.Fill"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Belirtilen şekil için dolgu biçimlendirme özelliklerini içeren bir FillFormat nesnesi döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/shape/fill/
---
## Shape.Fill property

Belirtilen şekil için dolgu biçimlendirme özelliklerini içeren bir [`FillFormat`](../fillformat/) nesnesi döndürür.

```csharp
public FillFormat Fill { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFillDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Şeklin doldurma formatını al
            FillFormat fillFmt = shape.Fill;

            // Renkli katı doldurma ayarlayın
            fillFmt.SolidFill.Color = System.Drawing.Color.Red;

            // Şeffaflığı ayarla
            fillFmt.Transparency = 0.5;

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeFillDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FillFormat](../../fillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


