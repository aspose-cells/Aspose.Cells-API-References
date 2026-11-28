---
title: "LineFormat.BeginArrowheadStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LineFormat property. Çizginin başlangıç ok tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/lineformat/beginarrowheadstyle/
---
## LineFormat.BeginArrowheadStyle property

Çizginin başlangıç ok tipini alır ve ayarlar.

```csharp
public MsoArrowheadStyle BeginArrowheadStyle { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir çizgi şekli ekleyin
            Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Başlangıç ok ucu stilini ayarla
            line.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Çalışma kitabını kaydedin
            workbook.Save("LineFormatPropertyBeginArrowheadStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


