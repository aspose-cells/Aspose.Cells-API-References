---
title: "TextEffectFormat.Text"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextEffectFormat. Le texte dans le WordArt"
type: docs
url: /fr/net/aspose.cells.drawing/texteffectformat/text/
---
## TextEffectFormat.Text property

Le texte dans le WordArt.

```csharp
public string Text { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyTextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter une forme d'effet de texte et définir son texte
            Shape shape = sheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 14, false, false, 0, 0, 0, 0, 100, 100);

            // Accéder et modifier la propriété texte de l'effet de texte
            shape.TextEffect.Text = "Updated Text";

            // Vérifier que le texte a été mis à jour
            Console.WriteLine("Text Effect Content: " + shape.TextEffect.Text);
        }
    }
}
```

### Voir aussi

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


