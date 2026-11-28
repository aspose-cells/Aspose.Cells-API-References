---
title: "LineFormat.EndArrowheadWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LineFormat özelliği. Çizginin son ok genişliği tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/lineformat/endarrowheadwidth/
---
## LineFormat.EndArrowheadWidth property

Çizginin bitiş ok genişliği tipini alır ve ayarlar.

```csharp
public MsoArrowheadWidth EndArrowheadWidth { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir çizgi şekli ekleyin
            Shape line = worksheet.Shapes.AddLine(10, 10, 100, 10, 5, 5);

            // Çizgi biçimini alın
            LineFormat lineFmt = line.Line;

            // Son ok genişliğini ayarlayın
            lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;

            // Çalışma kitabını kaydedin
            workbook.Save("LineFormatPropertyEndArrowheadWidthDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


