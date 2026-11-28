---
title: "LineFormat.BeginArrowheadLength"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LineFormat property. Çizginin başlangıç ok uzunluğu tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/lineformat/beginarrowheadlength/
---
## LineFormat.BeginArrowheadLength property

Çizginin başlangıç ok uzunluğu tipini alır ve ayarlar.

```csharp
public MsoArrowheadLength BeginArrowheadLength { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir çizgi şekli ekleyin
            Shape lineShape = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);
            LineShape line = (LineShape)lineShape;

            // Başlangıç ok ucu uzunluğunu ayarla
            line.Line.BeginArrowheadLength = MsoArrowheadLength.Long;

            // Çalışma kitabını kaydedin
            workbook.Save("LineFormatPropertyBeginArrowheadLengthDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


