---
title: "LineFormat.JoinType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LineFormat property. Çizgi birleşim tipini belirtir"
type: docs
url: /tr/net/aspose.cells.drawing/lineformat/jointype/
---
## LineFormat.JoinType property

Çizgi birleşim tipini belirtir.

```csharp
public LineJoinType JoinType { get; set; }
```

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyJoinTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir çizgi şekli oluştur
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Çizgi birleşim tipini Yuvarlak olarak ayarla
            line.Line.JoinType = LineJoinType.Round;

            // Çalışma kitabını kaydedin
            workbook.Save("LineJoinTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [LineJoinType](../../linejointype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


