---
title: "Shape.Line"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Çizgi stilini alır"
type: docs
url: /tr/net/aspose.cells.drawing/shape/line/
---
## Shape.Line property

Satır stilini alır

```csharp
public LineFormat Line { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLineDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir çizgi şekli ekleyin (LineShape'i doğrudan döndürür)
            LineShape lineShape = worksheet.Shapes.AddLine(1, 0, 1, 0, 5, 100);

            // Çizgi özelliklerine erişin ve değiştirin
            LineFormat lineFormat = lineShape.Line;
            lineFormat.CompoundType = MsoLineStyle.ThickThin;
            lineFormat.DashStyle = MsoLineDashStyle.DashDot;
            lineFormat.Weight = 3.0;
            lineFormat.BeginArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineFormat.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Çalışma kitabını kaydedin
            workbook.Save("LineShapeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [LineFormat](../../lineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


