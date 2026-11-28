---
title: "ShapeTextAlignment.TextHorizontalOverflow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeTextAlignment özelliği. Metin kutusunun yatay taşma tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.texts/shapetextalignment/texthorizontaloverflow/
---
## ShapeTextAlignment.TextHorizontalOverflow property

Metin kutusunun metin yatay taşma türünü alır ve ayarlar.

```csharp
public TextOverflowType TextHorizontalOverflow { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextHorizontalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir metin kutusu şekli ekle
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 50);
            textBox.Text = "This is a long text that demonstrates horizontal overflow behavior";

            // Yatay taşmayı Clip olarak ayarlayın
            textBox.TextBody.TextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;

            // Çalışma kitabını kaydedin
            workbook.Save("TextHorizontalOverflowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextOverflowType](../../../aspose.cells.drawing/textoverflowtype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


