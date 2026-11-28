---
title: "ShapeTextAlignment.IsAutoMargin"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeTextAlignment özelliği. Metin çerçevesinin marjının otomatik olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing.texts/shapetextalignment/isautomargin/
---
## ShapeTextAlignment.IsAutoMargin property

Metin çerçevesinin kenar boşluğunun otomatik olup olmadığını gösterir.

```csharp
public bool IsAutoMargin { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyIsAutoMarginDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Metin hizalamasına erişin ve IsAutoMargin özelliğini ayarlayın
            shape.TextBody.TextAlignment.IsAutoMargin = true;

            // Gösterim için bazı metinler ayarlayın
            shape.Text = "Sample text with auto margins";

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeTextAlignmentIsAutoMarginDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


