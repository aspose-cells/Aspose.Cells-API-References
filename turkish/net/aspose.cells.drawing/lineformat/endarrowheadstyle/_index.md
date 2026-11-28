---
title: "LineFormat.EndArrowheadStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LineFormat özelliği. Çizginin son ok tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/lineformat/endarrowheadstyle/
---
## LineFormat.EndArrowheadStyle property

Çizginin bitiş ok tipini alır ve ayarlar.

```csharp
public MsoArrowheadStyle EndArrowheadStyle { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir çizgi şekli ekleyin
            Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Çizgi biçimini alın
            LineFormat lineFmt = line.Line;

            // Son ok stilini ayarla
            lineFmt.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Çalışma kitabını kaydedin
            workbook.Save("LineFormatPropertyEndArrowheadStyleDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


