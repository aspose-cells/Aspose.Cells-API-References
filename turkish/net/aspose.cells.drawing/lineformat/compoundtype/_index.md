---
title: "LineFormat.CompoundType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LineFormat özelliği. Çizgi birleşik tipini belirtir"
type: docs
url: /tr/net/aspose.cells.drawing/lineformat/compoundtype/
---
## LineFormat.CompoundType property

Çizgi bileşik tipini belirtir.

```csharp
public MsoLineStyle CompoundType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyCompoundTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir çizgi şekli ekleyin
            Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);

            // Çizgi biçimini alın
            LineFormat lineFmt = line.Line;

            // Bileşik türü ayarla
            lineFmt.CompoundType = MsoLineStyle.Single;

            // Çalışma kitabını kaydedin
            workbook.Save("LineFormatCompoundTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [MsoLineStyle](../../msolinestyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


