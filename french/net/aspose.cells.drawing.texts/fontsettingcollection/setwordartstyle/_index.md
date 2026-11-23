---
title: "FontSettingCollection.SetWordArtStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FontSettingCollection. Définit le style WordArt prédéfini"
type: docs
url: /fr/net/aspose.cells.drawing.texts/fontsettingcollection/setwordartstyle/
---
## FontSettingCollection.SetWordArtStyle method

Définit le style WordArt prédéfini.

```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| style | PresetWordArtStyle | Le style WordArt prédéfini. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodSetWordArtStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Définir le texte initial
            fontSettingCollection.Text = "Sample Text for WordArt Styling";

            try
            {
                // Appeler la méthode SetWordArtStyle avec WordArtStyle7 (Remplissage en dégradé - Bleu, Accent 1, Réflexion)
                fontSettingCollection.SetWordArtStyle(PresetWordArtStyle.WordArtStyle7);

                Console.WriteLine("WordArt style applied successfully to the text box.");

                // Enregistrer le classeur pour montrer l'effet
                workbook.Save("FontSettingCollectionSetWordArtStyleDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetWordArtStyle method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


