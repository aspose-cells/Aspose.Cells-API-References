---
title: "TextBoxOptions.ShapeTextDirection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextBoxOptions özelliği. Belirli bir metin gövdesi içinde metin görüntüleme yönünü alır veya ayarlar. Excel'de Format Shape  Text Options  Text Box  Text direction ile eşdeğerdir"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textboxoptions/shapetextdirection/
---
## TextBoxOptions.ShapeTextDirection property

Belirli bir metin gövdesi içinde metin görüntüleme yönünü alır veya ayarlar. Excel'de "Format Shape - Text Options - Text Box - Text direction" ile eşdeğerdir

```csharp
public TextVerticalType ShapeTextDirection { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyShapeTextDirectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir metin kutusu şekli ekle
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);

            // Metin yönünü dikey olarak ayarla
            shape.TextBoxOptions.ShapeTextDirection = TextVerticalType.Vertical;

            // Yönü göstermek için bazı metinler ayarla
            shape.Text = "Vertical Text Example";

            // Çalışma kitabını kaydedin
            workbook.Save("TextBoxTextDirectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextVerticalType](../../textverticaltype/)
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


