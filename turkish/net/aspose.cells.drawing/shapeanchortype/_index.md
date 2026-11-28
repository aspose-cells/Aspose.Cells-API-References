---
title: "Enum ShapeAnchorType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ShapeAnchorType enum. Bağlama tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shapeanchortype/
---
## ShapeAnchorType enumeration

Bağlantı türünü temsil eder.

```csharp
public enum ShapeAnchorType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| TwoCellAnchor | `0` | İki hücreli bağlama yer tutucusunu temsil eder |
| OneCellAnchor | `1` | Tek hücreli bağlama yer tutucusunu temsil eder |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapeAnchorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grup kutusu şekli ekle
            Shape box = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 300, 250);
            box.Text = "Sample Group Box";
            
            // ShapeAnchorType kullanımını göster
            box.AnchorType = ShapeAnchorType.TwoCellAnchor;
            box.UpperLeftRow = 2;
            box.UpperLeftColumn = 1;
            box.LowerRightRow = 8;
            box.LowerRightColumn = 4;

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeAnchorTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


