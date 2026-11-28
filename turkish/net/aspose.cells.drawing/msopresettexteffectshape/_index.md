---
title: "Enum MsoPresetTextEffectShape"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.MsoPresetTextEffectShape enum. WordArt için önceden tanımlı metin efekti şekil tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/msopresettexteffectshape/
---
## MsoPresetTextEffectShape enumeration

WordArt'ın ön ayarlı metin efekti şekil tipini temsil eder.

```csharp
public enum MsoPresetTextEffectShape
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| PlainText | `136` | DüzMetin |
| Stop | `137` | Dur |
| TriangleUp | `138` | ÜçgenYukarı |
| TriangleDown | `139` | ÜçgenAşağı |
| ChevronUp | `140` | ŞeritYukarı |
| ChevronDown | `141` | ŞeritAşağı |
| RingInside | `142` | Halkaİç |
| RingOutside | `143` | HalkaDış |
| ArchUpCurve | `144` | KemerYukarıEğri |
| ArchDownCurve | `145` | KemerAşağıEğri |
| CircleCurve | `146` | DaireEğri |
| ButtonCurve | `147` | DüğmeEğri |
| ArchUpPour | `148` | KemerYukarıDök |
| ArchDownPour | `149` | KemerAşağıDök |
| CirclePour | `150` | DaireDök |
| ButtonPour | `151` | DüğmeDök |
| CurveUp | `152` | EğriYukarı |
| CurveDown | `153` | EğriAşağı |
| CanUp | `174` | KutuYukarı |
| CanDown | `175` | KutuAşağı |
| Wave1 | `156` | Dalga1 |
| Wave2 | `157` | Dalga2 |
| DoubleWave1 | `158` | ÇiftDalga1 |
| DoubleWave2 | `159` | ÇiftDalga2 |
| Inflate | `160` | Şişir |
| Deflate | `161` | Deflate |
| InflateBottom | `162` | InflateBottom |
| DeflateBottom | `163` | DeflateBottom |
| InflateTop | `164` | InflateTop |
| DeflateTop | `165` | DeflateTop |
| DeflateInflate | `166` | DeflateInflate |
| DeflateInflateDeflate | `167` | DeflateInflateDeflate |
| FadeRight | `168` | FadeRight |
| FadeLeft | `169` | FadeLeft |
| FadeUp | `170` | FadeUp |
| FadeDown | `171` | FadeDown |
| SlantUp | `172` | SlantUp |
| SlantDown | `173` | SlantDown |
| CascadeUp | `154` | CascadeUp |
| CascadeDown | `155` | CascadeDown |
| Mixed | `255` | Karışık |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoPresetTextEffectShapeDemo
    {
        public static void MsoPresetTextEffectShapeExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // WordArt metin efekti şekli ekleme
            shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
            TextEffectFormat textEffectFormat = shapes[0].TextEffect;

            // Ön ayarlı şekil tipini ayarlama
            textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpCurve;

            // Çalışma kitabını kaydedin
            workbook.Save("MsoPresetTextEffectShapeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


