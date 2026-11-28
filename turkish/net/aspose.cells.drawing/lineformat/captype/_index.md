---
title: "LineFormat.CapType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LineFormat property. Bitiş kapaklarını belirtir"
type: docs
url: /tr/net/aspose.cells.drawing/lineformat/captype/
---
## LineFormat.CapType property

Bitiş kapaklarını belirtir.

```csharp
public LineCapType CapType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyCapTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir çizgi şekli ekleyin
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Çizgi formatı özelliklerini ayarla
            LineFormat lineFmt = line.Line;
            lineFmt.CapType = LineCapType.Flat;

            // Çalışma kitabını kaydedin
            workbook.Save("LineFormatCapTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [LineCapType](../../linecaptype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


