---
title: "TextEffectFormat.SetTextEffect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode TextEffectFormat. Définit l'effet de texte prédéfini"
type: docs
url: /fr/net/aspose.cells.drawing/texteffectformat/settexteffect/
---
## TextEffectFormat.SetTextEffect method

Définit l'effet de texte prédéfini.

```csharp
public void SetTextEffect(MsoPresetTextEffect effect)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| effet | MsoPresetTextEffect | L'effet de texte prédéfini. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextEffectFormatMethodSetTextEffectWithMsoPresetTextEffectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour WordArt
            Shape wordArt = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", "Arial", 36, false, false, 0, 0, 0, 0, 100, 100);

            // Obtenir le TextEffectFormat de la forme
            TextEffectFormat textEffectFormat = wordArt.TextEffect;

            try
            {
                // Appeler la méthode SetTextEffect avec le paramètre MsoPresetTextEffect
                textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);

                // Définir des propriétés supplémentaires pour le WordArt
                textEffectFormat.FontBold = true;
                textEffectFormat.FontItalic = false;
                textEffectFormat.FontSize = 24;

                Console.WriteLine("SetTextEffect method executed successfully with MsoPresetTextEffect.TextEffect10");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextEffect method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("TextEffectFormatMethodSetTextEffectWithMsoPresetTextEffectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


