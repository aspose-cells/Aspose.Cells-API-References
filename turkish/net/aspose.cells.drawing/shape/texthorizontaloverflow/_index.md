---
title: "Shape.TextHorizontalOverflow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Metin içeren şeklin metin yatay taşma tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/texthorizontaloverflow/
---
## Shape.TextHorizontalOverflow property

Metin içeren şeklin metin yatay taşma türünü alır ve ayarlar.

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
    public class ShapePropertyTextHorizontalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir metin kutusu şekli ekleyin
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            textBox.Text = "This is a long text that will demonstrate text horizontal overflow functionality";

            // İlk taşma tipini Clip olarak ayarlayın
            textBox.TextHorizontalOverflow = TextOverflowType.Clip;
            Console.WriteLine("TextHorizontalOverflow set to Clip (text will be clipped)");

            // Taşma tipini Overflow olarak değiştirin
            textBox.TextHorizontalOverflow = TextOverflowType.Overflow;
            Console.WriteLine("TextHorizontalOverflow changed to Overflow (text will overflow)");

            // Çalışma kitabını kaydedin
            workbook.Save("TextHorizontalOverflowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextOverflowType](../../textoverflowtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


