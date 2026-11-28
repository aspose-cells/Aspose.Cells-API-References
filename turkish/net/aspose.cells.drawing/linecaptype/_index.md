---
title: "Enum LineCapType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.LineCapType enum. Bir çizginin uç kapaklarını temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/linecaptype/
---
## LineCapType enumeration

Bir çizginin uçlarını temsil eder

```csharp
public enum LineCapType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Square | `0` | Kare, çizgi genişliğinin yarısı kadar dışarı çıkar. |
| Round | `1` | Yuvarlak uçlar. |
| Flat | `2` | Çizgi son noktada biter. |
| None | `3` | Kap yok |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassLineCapTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);
            
            LineFormat lineFmt = shape.Line;
            lineFmt.CapType = LineCapType.Flat;
            lineFmt.Weight = 2.0;
            lineFmt.DashStyle = MsoLineDashStyle.Solid;
            
            workbook.Save("LineCapTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


