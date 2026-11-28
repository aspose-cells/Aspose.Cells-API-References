---
title: "Shape.Text"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Bu şeklin metnini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/text/
---
## Shape.Text property

Bu şeklin metnini alır ve ayarlar.

```csharp
public string Text { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Metni null ise ayarla
            if (shape.Text == null)
            {
                shape.Text = "This is a test.";
            }

            // Metni değiştir
            shape.Text = "Updated text demo";

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeTextDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


