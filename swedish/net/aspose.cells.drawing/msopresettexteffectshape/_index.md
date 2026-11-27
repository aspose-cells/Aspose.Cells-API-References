---
title: "Enum MsoPresetTextEffectShape"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.MsoPresetTextEffectShape-enum. Representerar förinställd texteffektformtyp för WordArt"
type: docs
url: /sv/net/aspose.cells.drawing/msopresettexteffectshape/
---
## MsoPresetTextEffectShape enumeration

Representerar förinställd texteffektformtyp för WordArt.

```csharp
public enum MsoPresetTextEffectShape
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| PlainText | `136` | PlainText |
| Stop | `137` | Stopp |
| TriangleUp | `138` | TriangleUp |
| TriangleDown | `139` | TriangleDown |
| ChevronUp | `140` | ChevronUp |
| ChevronDown | `141` | ChevronDown |
| RingInside | `142` | RingInside |
| RingOutside | `143` | RingOutside |
| ArchUpCurve | `144` | ArchUpCurve |
| ArchDownCurve | `145` | ArchDownCurve |
| CircleCurve | `146` | CircleCurve |
| ButtonCurve | `147` | KnappKurva |
| ArchUpPour | `148` | BågeUppHäll |
| ArchDownPour | `149` | BågeNedHäll |
| CirclePour | `150` | CirkelHäll |
| ButtonPour | `151` | KnappHäll |
| CurveUp | `152` | KurvaUpp |
| CurveDown | `153` | KurvaNed |
| CanUp | `174` | BurkUpp |
| CanDown | `175` | BurkNed |
| Wave1 | `156` | Våg1 |
| Wave2 | `157` | Våg2 |
| DoubleWave1 | `158` | DubbelVåg1 |
| DoubleWave2 | `159` | DubbelVåg2 |
| Inflate | `160` | FyllUpp |
| Deflate | `161` | Töm |
| InflateBottom | `162` | FyllUppNederst |
| DeflateBottom | `163` | TömNederst |
| InflateTop | `164` | FyllUppÖverst |
| DeflateTop | `165` | TömÖverst |
| DeflateInflate | `166` | TömFyllUpp |
| DeflateInflateDeflate | `167` | TömFyllUppTöm |
| FadeRight | `168` | TonaHöger |
| FadeLeft | `169` | TonaVänster |
| FadeUp | `170` | TonaUpp |
| FadeDown | `171` | TonaNed |
| SlantUp | `172` | SlantUp |
| SlantDown | `173` | SlantDown |
| CascadeUp | `154` | CascadeUp |
| CascadeDown | `155` | CascadeDown |
| Mixed | `255` | Blandad |

### Exempel

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
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Lägger till en WordArt-texteffektform
            shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
            TextEffectFormat textEffectFormat = shapes[0].TextEffect;

            // Ställer in den förinställda formtypen
            textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpCurve;

            // Spara arbetsboken
            workbook.Save("MsoPresetTextEffectShapeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


