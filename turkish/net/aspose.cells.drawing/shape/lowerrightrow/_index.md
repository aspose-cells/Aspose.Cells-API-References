---
title: "Shape.LowerRightRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Alt sağ köşe satır indeksini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/lowerrightrow/
---
## Shape.LowerRightRow property

Alt sağ köşe satır indeksini temsil eder.

```csharp
public int LowerRightRow { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLowerRightRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // LowerRightRow özelliğini ayarla ve göster
            Console.WriteLine("Original LowerRightRow: " + shape.LowerRightRow);
            shape.LowerRightRow = 3;
            Console.WriteLine("Modified LowerRightRow: " + shape.LowerRightRow);

            // Test durumuna göre koşullu değişiklik
            if (shape.LowerRightRow == 3)
            {
                shape.LowerRightRow = 1;
                Console.WriteLine("Final LowerRightRow after condition: " + shape.LowerRightRow);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


