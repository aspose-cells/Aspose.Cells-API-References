---
title: "Enum BevelType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.BevelType enum. 3B'de bir şekle uygulanabilen bir kenar tipi için ön ayarı temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/beveltype/
---
## BevelType enumeration

3B'de bir şekle uygulanabilen bir köşe tipi için bir ön ayarı temsil eder.

```csharp
public enum BevelType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Kenarsız |
| Angle | `1` | Açı |
| ArtDeco | `2` | Art deco |
| Circle | `3` | Daire |
| Convex | `4` | Konveks |
| CoolSlant | `5` | Serin eğim |
| Cross | `6` | Çapraz |
| Divot | `7` | Çökük |
| HardEdge | `8` | Keskin kenar |
| RelaxedInset | `9` | Rahat iç kenar |
| Riblet | `10` | Kaburga |
| Slope | `11` | Eğim |
| SoftRound | `12` | Yumuşak yuvarlak |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class BevelTypeDemo
    {
        public static void BevelTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 100);

            // Şeklin 3B biçimine eriş
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Üst köşe tipi ve boyutlarını ayarlayın
            threeDFormat.TopBevelType = BevelType.SoftRound;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;

            // Alt köşe tipi ve boyutlarını ayarlayın
            threeDFormat.BottomBevelType = BevelType.Divot;
            threeDFormat.BottomBevelWidth = 5;
            threeDFormat.BottomBevelHeight = 5;

            // Çalışma kitabını kaydedin
            workbook.Save("BevelTypeExample.xlsx");
            workbook.Save("BevelTypeExample.pdf");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


