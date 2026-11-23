---
title: "Classe TextEffectFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.TextEffectFormat. Contient les propriétés et méthodes qui s'appliquent aux objets WordArt"
type: docs
url: /fr/net/aspose.cells.drawing/texteffectformat/
---
## TextEffectFormat class

Contient des propriétés et des méthodes qui s'appliquent aux objets WordArt.

```csharp
public class TextEffectFormat
```

## Propriétés

| Nom | Description |
| --- | --- |
| [FontBold](../../aspose.cells.drawing/texteffectformat/fontbold/) { get; set; } | Indique si la police est en gras. |
| [FontItalic](../../aspose.cells.drawing/texteffectformat/fontitalic/) { get; set; } | Indique si la police est en italique. |
| [FontName](../../aspose.cells.drawing/texteffectformat/fontname/) { get; set; } | Le nom de la police utilisée dans le WordArt. |
| [FontSize](../../aspose.cells.drawing/texteffectformat/fontsize/) { get; set; } | La taille (en points) de la police utilisée dans le WordArt. |
| [PresetShape](../../aspose.cells.drawing/texteffectformat/presetshape/) { get; set; } | Obtient et définit le type de forme prédéfini. |
| [RotatedChars](../../aspose.cells.drawing/texteffectformat/rotatedchars/) { get; set; } | Si vrai, les caractères du WordArt spécifié sont pivotés de 90 degrés par rapport à la forme englobante du WordArt. |
| [Text](../../aspose.cells.drawing/texteffectformat/text/) { get; set; } | Le texte dans le WordArt. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetTextEffect](../../aspose.cells.drawing/texteffectformat/settexteffect/)(MsoPresetTextEffect) | Définit l'effet de texte prédéfini. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTextEffectFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            
            // Ajouter une forme d'effet de texte
            shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
            
            // Modifier l'effet de texte
            TextEffectFormat textEffectFormat = shapes[0].TextEffect;
            textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);
            
            // Enregistrez le classeur
            workbook.Save("TextEffectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


