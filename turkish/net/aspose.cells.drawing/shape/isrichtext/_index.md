---
title: "Shape.IsRichText"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Metnin zengin metin olup olmadığı"
type: docs
url: /tr/net/aspose.cells.drawing/shape/isrichtext/
---
## Shape.IsRichText property

Metnin zengin metin olup olmadığı.

```csharp
public bool IsRichText { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsRichTextDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Metin içeren bir şekil ekleyin
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "This is <b>rich</b> text";

            // Metnin zengin metin olup olmadığını kontrol edin
            if (shape.IsRichText)
            {
                Console.WriteLine("The text is rich text.");
            }
            else
            {
                Console.WriteLine("The text is not rich text.");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


