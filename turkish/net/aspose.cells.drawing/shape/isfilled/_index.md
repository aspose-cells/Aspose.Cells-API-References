---
title: "Shape.IsFilled"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Doldurma biçiminin görünür olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/shape/isfilled/
---
## Shape.IsFilled property

Dolgu biçiminin görünür olup olmadığını gösterir.

```csharp
public bool IsFilled { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsFilledDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // IsFilled özelliğini kontrol et ve değiştir
            if (shape.IsFilled == false)
            {
                shape.IsFilled = true;
                shape.FillFormat.ForeColor = System.Drawing.Color.Red;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeIsFilledDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


