---
title: "Shape.LinkedCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Kontrolün değerine bağlı çalışma sayfası aralığını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/linkedcell/
---
## Shape.LinkedCell property

Denetimin değerine bağlı çalışma sayfası aralığını alır veya ayarlar.

```csharp
public string LinkedCell { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLinkedCellDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // LinkedCell özelliğini B6'ya ayarla
            shape.LinkedCell = "$B$6";

            // LinkedCell B6 ise A1'e değiştir
            if (shape.LinkedCell.Equals("$B$6"))
            {
                shape.LinkedCell = "A1";
            }

            // Mevcut LinkedCell değerini çıktı olarak ver
            Console.WriteLine("Shape's LinkedCell: " + shape.LinkedCell);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


