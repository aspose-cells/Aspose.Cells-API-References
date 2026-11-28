---
title: "Enum MsoArrowheadStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.MsoArrowheadStyle enum. Şekil kenar çizgisinin uç tipini tanımlar"
type: docs
url: /tr/net/aspose.cells.drawing/msoarrowheadstyle/
---
## MsoArrowheadStyle enumeration

Şekil kenarlık çizgisinin uç tipini listeler.

```csharp
public enum MsoArrowheadStyle
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Uç tipi yok. |
| Arrow | `1` | Ok uç tipi. |
| ArrowStealth | `2` | Gizli ok uç tipi. |
| ArrowDiamond | `3` | Elmas ok uç tipi. |
| ArrowOval | `4` | Oval ok uç tipi. |
| ArrowOpen | `5` | Açık ok uç tipi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassMsoArrowheadStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir çizgi şekli ekleyin
            LineShape lineShape = worksheet.Shapes.AddLine(5, 5, 10, 10, 100, 100);

            // Çizgi özelliklerini ayarlayın
            MsoLineFormat lineFormat = lineShape.LineFormat;
            lineFormat.ForeColor = System.Drawing.Color.Black;
            lineFormat.DashStyle = MsoLineDashStyle.DashDot;
            lineFormat.Weight = 0.75;

            // Ok ucu stillerini ayarlayın
            lineShape.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowStealth;
            lineShape.Line.EndArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineShape.Line.BeginArrowheadLength = MsoArrowheadLength.Medium;
            lineShape.Line.EndArrowheadLength = MsoArrowheadLength.Medium;

            // Çalışma kitabını kaydedin
            workbook.Save("MsoArrowheadStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


