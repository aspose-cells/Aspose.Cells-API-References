---
title: "Shape.TextDirection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Bu nesnenin metin akış yönünü alır/ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/textdirection/
---
## Shape.TextDirection property

Bu nesne için metin akış yönünü alır/ayarlar.

```csharp
public TextDirectionType TextDirection { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir metin kutusu şekli ekle
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
            shape.Text = "Sample Text";

            // TextDirection özelliğini ayarlayın ve gösterin
            shape.TextDirection = TextDirectionType.Context;
            Console.WriteLine("Initial TextDirection: " + shape.TextDirection);

            // Metin yönünü değiştirin
            shape.TextDirection = TextDirectionType.LeftToRight;
            Console.WriteLine("Updated TextDirection: " + shape.TextDirection);

            // Çalışma kitabını kaydedin
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


