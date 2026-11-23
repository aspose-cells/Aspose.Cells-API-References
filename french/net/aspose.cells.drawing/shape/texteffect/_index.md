---
title: "Shape.TextEffect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Retourne un objet TextEffectFormat qui contient les propriétés de mise en forme texteffect pour la forme spécifiée. S'applique aux objets Shape qui représentent WordArt"
type: docs
url: /fr/net/aspose.cells.drawing/shape/texteffect/
---
## Shape.TextEffect property

Renvoie un objet TextEffectFormat qui contient les propriétés de formatage d'effet de texte pour la forme spécifiée. S'applique aux objets Shape qui représentent du WordArt.

```csharp
public TextEffectFormat TextEffect { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextEffectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme WordArt avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "Sample Text", 10, 10, 200, 50, 0, 0);

            // Vérifiez s'il s'agit de WordArt et accédez aux propriétés TextEffect
            if (shape.IsWordArt)
            {
                TextEffectFormat textEffectFormat = shape.TextEffect;
                textEffectFormat.FontBold = true;
                textEffectFormat.FontItalic = true;
                textEffectFormat.FontName = "Arial";
                textEffectFormat.FontSize = 14;
            }

            // Enregistrez le classeur
            workbook.Save("TextEffectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextEffectFormat](../../texteffectformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


