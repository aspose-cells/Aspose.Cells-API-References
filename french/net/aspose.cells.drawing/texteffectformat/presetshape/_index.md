---
title: "TextEffectFormat.PresetShape"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextEffectFormat. Obtient et définit le type de forme prédéfini"
type: docs
url: /fr/net/aspose.cells.drawing/texteffectformat/presetshape/
---
## TextEffectFormat.PresetShape property

Obtient et définit le type de forme prédéfini.

```csharp
public MsoPresetTextEffectShape PresetShape { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyPresetShapeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme avec effet de texte
            Shape shape = worksheet.Shapes.AddTextEffect(
                MsoPresetTextEffect.TextEffect1,
                "Sample Text",
                "Arial",
                18,
                false,
                false,
                0,
                0,
                100,
                200,
                0,
                0);

            // Obtenir le format d'effet de texte
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // Définir et obtenir la propriété PresetShape
            textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpPour;
            Console.WriteLine("PresetShape: " + textEffectFormat.PresetShape);

            // Modifier d'autres propriétés
            textEffectFormat.Text = "Updated Text";
            textEffectFormat.FontBold = true;
            textEffectFormat.FontSize = 24;

            // Enregistrez le classeur
            workbook.Save("TextEffectFormatDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [MsoPresetTextEffectShape](../../msopresettexteffectshape/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


