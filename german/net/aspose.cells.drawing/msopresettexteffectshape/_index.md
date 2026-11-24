---
title: "Enum MsoPresetTextEffectShape"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.MsoPresetTextEffectShape Enum. Stellt den voreingestellten Text‑Effekt‑Formtyp von WordArt dar"
type: docs
url: /de/net/aspose.cells.drawing/msopresettexteffectshape/
---
## MsoPresetTextEffectShape enumeration

Stellt den voreingestellten Formen‑Typ des Texteffekts von WordArt dar.

```csharp
public enum MsoPresetTextEffectShape
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| PlainText | `136` | PlainText |
| Stop | `137` | Stopp |
| TriangleUp | `138` | DreieckOben |
| TriangleDown | `139` | DreieckUnten |
| ChevronUp | `140` | ChevronOben |
| ChevronDown | `141` | ChevronUnten |
| RingInside | `142` | RingInnen |
| RingOutside | `143` | RingAußen |
| ArchUpCurve | `144` | BogenAufwärtsKurve |
| ArchDownCurve | `145` | BogenAbwärtsKurve |
| CircleCurve | `146` | KreisKurve |
| ButtonCurve | `147` | KnopfKurve |
| ArchUpPour | `148` | BogenAufwärtsGießen |
| ArchDownPour | `149` | BogenAbwärtsGießen |
| CirclePour | `150` | KreisGießen |
| ButtonPour | `151` | SchaltflächeGießen |
| CurveUp | `152` | KurveAuf |
| CurveDown | `153` | KurveAb |
| CanUp | `174` | DoseAuf |
| CanDown | `175` | DoseAb |
| Wave1 | `156` | Welle1 |
| Wave2 | `157` | Welle2 |
| DoubleWave1 | `158` | DoppelteWelle1 |
| DoubleWave2 | `159` | DoppelteWelle2 |
| Inflate | `160` | Aufblasen |
| Deflate | `161` | Entleeren |
| InflateBottom | `162` | AufblasenUnten |
| DeflateBottom | `163` | EntleerenUnten |
| InflateTop | `164` | AufblasenOben |
| DeflateTop | `165` | EntleerenOben |
| DeflateInflate | `166` | EntleerenAufblasen |
| DeflateInflateDeflate | `167` | EntleerenAufblasenEntleeren |
| FadeRight | `168` | VerblassenRechts |
| FadeLeft | `169` | VerblassenLinks |
| FadeUp | `170` | VerblassenOben |
| FadeDown | `171` | VerblassenUnten |
| SlantUp | `172` | SchrägAuf |
| SlantDown | `173` | SchrägAb |
| CascadeUp | `154` | KaskadeAuf |
| CascadeDown | `155` | CascadeDown |
| Mixed | `255` | Gemischt |

### Beispiele

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
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Hinzufügen einer WordArt-Text-Effektform
            shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
            TextEffectFormat textEffectFormat = shapes[0].TextEffect;

            // Festlegen des voreingestellten Formtyps
            textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpCurve;

            // Speichere die Arbeitsmappe
            workbook.Save("MsoPresetTextEffectShapeExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


