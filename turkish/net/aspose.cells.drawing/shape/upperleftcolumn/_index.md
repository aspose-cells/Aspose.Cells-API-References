---
title: "Shape.UpperLeftColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Üst sol köşe sütun indeksini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/upperleftcolumn/
---
## Shape.UpperLeftColumn property

Üst sol köşe sütun indeksini temsil eder.

```csharp
public int UpperLeftColumn { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperLeftColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 100, 100, 100);

            // UpperLeftColumn özelliğini ayarla ve göster
            shape.UpperLeftColumn = 3;
            Console.WriteLine("Shape's initial leftColumn: " + shape.UpperLeftColumn);

            // UpperLeftColumn değerini değiştir
            if (shape.UpperLeftColumn == 3)
            {
                shape.UpperLeftColumn = 1;
                Console.WriteLine("Shape's modified leftColumn: " + shape.UpperLeftColumn);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeUpperLeftColumnDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


