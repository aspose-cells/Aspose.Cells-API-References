---
title: "PresetShadowType enumı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.PresetShadowType enumı. Önceden tanımlı gölge tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/presetshadowtype/
---
## PresetShadowType enumeration

Ön ayarlı gölge tipini temsil eder.

```csharp
public enum PresetShadowType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| NoShadow | `0` | Gölge yok. |
| Custom | `1` | Özel gölge. |
| OffsetDiagonalBottomRight | `2` | Dış gölge ofseti çapraz alt sağ. |
| OffsetBottom | `3` | Dış gölge ofseti alt. |
| OffsetDiagonalBottomLeft | `4` | Dış gölge ofseti çapraz alt sol. |
| OffsetRight | `5` | Dış gölge ofseti sağ. |
| OffsetCenter | `6` | Dış gölge ofseti merkez. |
| OffsetLeft | `7` | Dış gölge ofseti sol. |
| OffsetDiagonalTopRight | `8` | Dış gölge ofseti çapraz üst sağ. |
| OffsetTop | `9` | Dış gölge ofseti üst. |
| OffsetDiagonalTopLeft | `10` | Dış gölge ofseti çapraz üst sol. |
| InsideDiagonalTopLeft | `11` | İç gölge iç çapraz üst sol. |
| InsideTop | `12` | İç gölge iç üst. |
| InsideDiagonalTopRight | `13` | İç gölge iç çapraz üst sağ. |
| InsideLeft | `14` | İç gölge iç sol. |
| InsideCenter | `15` | İç gölge iç merkez. |
| InsideRight | `16` | İç gölge iç sağ. |
| InsideDiagonalBottomLeft | `17` | İç gölge iç çapraz alt sol. |
| InsideBottom | `18` | İç gölge iç alt. |
| InsideDiagonalBottomRight | `19` | İç gölge iç çapraz alt sağ. |
| PerspectiveDiagonalUpperLeft | `20` | Dış gölge perspektif çapraz üst sol. |
| PerspectiveDiagonalUpperRight | `21` | Dış gölge perspektif çapraz üst sağ. |
| Below | `22` | Dış gölge aşağıda. |
| PerspectiveDiagonalLowerLeft | `23` | Dış gölge perspektif çapraz alt sol. |
| PerspectiveDiagonalLowerRight | `24` | Dış gölge perspektif çapraz alt sağ. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassPresetShadowTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gölge etkilerini göstermek için bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Farklı ön ayarlı gölge türlerini ayarla
            shape.ShadowEffect.PresetType = PresetShadowType.OffsetDiagonalBottomRight;
            Console.WriteLine("Shadow type set to: " + shape.ShadowEffect.PresetType);

            // Başka bir gölge türüne değiştir
            shape.ShadowEffect.PresetType = PresetShadowType.OffsetBottom;
            Console.WriteLine("Shadow type changed to: " + shape.ShadowEffect.PresetType);

            // Çalışma kitabını kaydedin
            workbook.Save("PresetShadowTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


