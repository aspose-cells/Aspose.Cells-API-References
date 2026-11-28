---
title: "Enum MirrorType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.MirrorType enum. Doku dolgusunun yansıtma tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/mirrortype/
---
## MirrorType enumeration

Doku doldurmanın yansıma tipini temsil eder

```csharp
public enum MirrorType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Yok |
| Horizonal | `1` | Yatay |
| Vertical | `2` | Dikey |
| Both | `3` | Her ikisi |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassMirrorTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // MirrorType'ı göstermek için bir şekil ekleyin
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 200);

            // Farklı yansıtma tipleriyle doku dolgu ayarlayın
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Horizonal;
            shape = worksheet.Shapes.AddRectangle(2, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Vertical;
            shape = worksheet.Shapes.AddRectangle(3, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Both;
            shape = worksheet.Shapes.AddRectangle(4, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.None;

            // Sonucu kaydet
            workbook.Save("MirrorTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


