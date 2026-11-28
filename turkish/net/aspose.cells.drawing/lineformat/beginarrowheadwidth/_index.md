---
title: "LineFormat.BeginArrowheadWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LineFormat özelliği. Çizginin başlangıç ok genişliği tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/lineformat/beginarrowheadwidth/
---
## LineFormat.BeginArrowheadWidth property

Çizginin başlangıç ok genişliği tipini alır ve ayarlar.

```csharp
public MsoArrowheadWidth BeginArrowheadWidth { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadWidthDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir çizgi şekli ekleyin
            Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 10);

            // Çizgi formatı özelliklerini ayarlayın
            LineFormat lineFmt = line.Line;
            lineFmt.BeginArrowheadWidth = MsoArrowheadWidth.Medium;
            lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;

            // Çalışma kitabını kaydedin
            workbook.Save("LineFormatDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


