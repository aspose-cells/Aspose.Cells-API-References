---
title: "TextEffectFormat.RotatedChars"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextEffectFormat. Si true, les caractères dans le WordArt spécifié sont tournés de 90 degrés par rapport à la forme englobante du WordArt"
type: docs
url: /fr/net/aspose.cells.drawing/texteffectformat/rotatedchars/
---
## TextEffectFormat.RotatedChars property

Si vrai, les caractères du WordArt spécifié sont pivotés de 90 degrés par rapport à la forme englobante du WordArt.

```csharp
public bool RotatedChars { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyRotatedCharsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme avec effet de texte
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 100, 100, 200, 50);

            // Obtenir le format d'effet de texte
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // Définir la propriété RotatedChars sur true
            textEffectFormat.RotatedChars = true;

            // Enregistrez le classeur
            workbook.Save("TextEffectFormat_RotatedChars_Output.xlsx");

            // Vérifier la propriété RotatedChars
            Console.WriteLine("RotatedChars property value: " + textEffectFormat.RotatedChars);
        }
    }
}
```

### Voir aussi

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


