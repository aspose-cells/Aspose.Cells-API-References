---
title: "Enum MsoPresetTextEffectShape"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.MsoPresetTextEffectShape enum. Représente le type de forme d'effet de texte prédéfini de WordArt"
type: docs
url: /fr/net/aspose.cells.drawing/msopresettexteffectshape/
---
## MsoPresetTextEffectShape enumeration

Représente le type de forme d’effet de texte prédéfini de WordArt.

```csharp
public enum MsoPresetTextEffectShape
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| PlainText | `136` | Texte brut |
| Stop | `137` | Arrêt |
| TriangleUp | `138` | TriangleHaut |
| TriangleDown | `139` | TriangleBas |
| ChevronUp | `140` | ChevronHaut |
| ChevronDown | `141` | ChevronBas |
| RingInside | `142` | AnneauIntérieur |
| RingOutside | `143` | AnneauExtérieur |
| ArchUpCurve | `144` | ArcHautCourbe |
| ArchDownCurve | `145` | ArcBasCourbe |
| CircleCurve | `146` | CercleCourbe |
| ButtonCurve | `147` | BoutonCourbe |
| ArchUpPour | `148` | ArcHautVerser |
| ArchDownPour | `149` | ArcBasVerser |
| CirclePour | `150` | CercleVerser |
| ButtonPour | `151` | BoutonVerser |
| CurveUp | `152` | CourbeHaut |
| CurveDown | `153` | CourbeBas |
| CanUp | `174` | CanetteHaut |
| CanDown | `175` | CanetteBas |
| Wave1 | `156` | Vague1 |
| Wave2 | `157` | Vague2 |
| DoubleWave1 | `158` | DoubleVague1 |
| DoubleWave2 | `159` | DoubleVague2 |
| Inflate | `160` | Gonfler |
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
| Mixed | `255` | Mixte |

### Exemples

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
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Ajout d'une forme d'effet de texte WordArt
            shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
            TextEffectFormat textEffectFormat = shapes[0].TextEffect;

            // Définition du type de forme prédéfini
            textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpCurve;

            // Enregistrez le classeur
            workbook.Save("MsoPresetTextEffectShapeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


