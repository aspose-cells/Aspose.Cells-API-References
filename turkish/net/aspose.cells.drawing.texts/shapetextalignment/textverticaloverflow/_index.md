---
title: "ShapeTextAlignment.TextVerticalOverflow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeTextAlignment özelliği. Metin kutusunun dikey taşma tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.texts/shapetextalignment/textverticaloverflow/
---
## ShapeTextAlignment.TextVerticalOverflow property

Metin kutusunun metin dikey taşma türünü alır ve ayarlar.

```csharp
public TextOverflowType TextVerticalOverflow { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextVerticalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);

            // Dikey olarak taşabilecek metni ayarlayın
            shape.Text = "This is a long text that might overflow vertically if not clipped properly";

            // Metin hizalamasını alın ve dikey taşmayı Kes olarak ayarlayın
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;

            // Çalışma kitabını kaydedin
            workbook.Save("TextVerticalOverflowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextOverflowType](../../../aspose.cells.drawing/textoverflowtype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


