---
title: "LineFormat.EndArrowheadLength"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LineFormat property. Çizginin son ok uzunluğu tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/lineformat/endarrowheadlength/
---
## LineFormat.EndArrowheadLength property

Çizginin bitiş ok uzunluğu tipini alır ve ayarlar.

```csharp
public MsoArrowheadLength EndArrowheadLength { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir çizgi şekli ekle ve şekil nesnesini doğrudan al
            LineShape line = (LineShape)worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 10);

            // Son ok ucu uzunluğunu ayarla
            line.Line.EndArrowheadLength = MsoArrowheadLength.Long;

            // Çalışma kitabını kaydedin
            workbook.Save("LineFormatPropertyEndArrowheadLengthDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


