---
title: "Shape.TextOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin metin seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/textoptions/
---
## Shape.TextOptions property

Şeklin metin seçeneklerini temsil eder.

```csharp
public TextOptions TextOptions { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Şekil için metin ayarlayın
            shape.Text = "Sample Text";

            // TextOptions'a erişin ve değiştirin
            TextOptions opt = shape.TextOptions;
            opt.Color = Color.Blue;
            opt.Size = 8;

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeTextOptionsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


