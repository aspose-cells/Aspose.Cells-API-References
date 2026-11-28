---
title: "Shape.WidthInShape"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Şekil özelliği. Şeklin genişliğini, üst şeklin 1/4000 biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/widthinshape/
---
## Shape.WidthInShape property

Şeklin genişliğini, ebeveyn şeklinin 1/4000 birimi cinsinden temsil eder.

```csharp
public int WidthInShape { get; set; }
```

### Açıklamalar

Yalnızca bu şekil grup veya grafik içinde olduğunda uygulanır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthInShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İki dikdörtgen şekil oluştur
            Shape rect1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            Shape rect2 = worksheet.Shapes.AddRectangle(0, 100, 0, 0, 100, 100);
            
            // Şekil nesnelerini kullanarak şekilleri grupla
            GroupShape group = worksheet.Shapes.Group(new Shape[] { rect1, rect2 });
            
            // WidthInShape kullanımını göster
            if (rect1.IsInGroup && rect1.WidthInShape == 2000)
            {
                rect1.WidthInShape = 4000;
            }
            
            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


