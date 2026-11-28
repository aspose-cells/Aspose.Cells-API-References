---
title: "Shape.ActualLowerRightRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Gerçek alt satırı al"
type: docs
url: /tr/net/aspose.cells.drawing/shape/actuallowerrightrow/
---
## Shape.ActualLowerRightRow property

Gerçek alt satırı al.

```csharp
public int ActualLowerRightRow { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyActualLowerRightRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek bir şekil ekle (dikdörtgen)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 100);

            // Şeklin gerçek alt sağ satırını al
            int actualLowerRightRow = shape.ActualLowerRightRow;

            // Sonucu çıktı olarak ver
            Console.WriteLine("Actual Lower Right Row of the shape: " + actualLowerRightRow);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


