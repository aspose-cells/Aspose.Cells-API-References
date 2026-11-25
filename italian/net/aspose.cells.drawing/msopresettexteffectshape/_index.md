---
title: "Enum MsoPresetTextEffectShape"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.MsoPresetTextEffectShape enum. Rappresenta il tipo di forma di effetto testo predefinito di WordArt"
type: docs
url: /it/net/aspose.cells.drawing/msopresettexteffectshape/
---
## MsoPresetTextEffectShape enumeration

Rappresenta il tipo di forma di effetto testo predefinito di WordArt.

```csharp
public enum MsoPresetTextEffectShape
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| PlainText | `136` | Testo semplice |
| Stop | `137` | Interrompi |
| TriangleUp | `138` | Triangolo verso l'alto |
| TriangleDown | `139` | Triangolo verso il basso |
| ChevronUp | `140` | Chevron verso l'alto |
| ChevronDown | `141` | Chevron verso il basso |
| RingInside | `142` | Anello interno |
| RingOutside | `143` | Anello esterno |
| ArchUpCurve | `144` | Arco curvo verso l'alto |
| ArchDownCurve | `145` | Arco curvo verso il basso |
| CircleCurve | `146` | Curva circolare |
| ButtonCurve | `147` | Curva pulsante |
| ArchUpPour | `148` | Versamento arco verso l'alto |
| ArchDownPour | `149` | Versamento arco verso il basso |
| CirclePour | `150` | Versamento circolare |
| ButtonPour | `151` | Versamento pulsante |
| CurveUp | `152` | Curva verso l'alto |
| CurveDown | `153` | Curva verso il basso |
| CanUp | `174` | Lattina verso l'alto |
| CanDown | `175` | Lattina verso il basso |
| Wave1 | `156` | Onda 1 |
| Wave2 | `157` | Onda 2 |
| DoubleWave1 | `158` | Doppia onda 1 |
| DoubleWave2 | `159` | Doppia onda 2 |
| Inflate | `160` | Gonfia |
| Deflate | `161` | Riduci |
| InflateBottom | `162` | Espandi in basso |
| DeflateBottom | `163` | Riduci in basso |
| InflateTop | `164` | Espandi in alto |
| DeflateTop | `165` | Riduci in alto |
| DeflateInflate | `166` | Riduci/Espandi |
| DeflateInflateDeflate | `167` | RiduciEspandiRiduci |
| FadeRight | `168` | Dissolvi a destra |
| FadeLeft | `169` | Dissolvi a sinistra |
| FadeUp | `170` | Dissolvi verso l'alto |
| FadeDown | `171` | Dissolvi verso il basso |
| SlantUp | `172` | Inclina verso l'alto |
| SlantDown | `173` | Inclina verso il basso |
| CascadeUp | `154` | Cascata verso l'alto |
| CascadeDown | `155` | Cascata verso il basso |
| Mixed | `255` | Mixed |

### Esempi

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
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Aggiunta di una forma effetto testo WordArt
            shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
            TextEffectFormat textEffectFormat = shapes[0].TextEffect;

            // Impostazione del tipo di forma predefinita
            textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpCurve;

            // Salva la cartella di lavoro
            workbook.Save("MsoPresetTextEffectShapeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


