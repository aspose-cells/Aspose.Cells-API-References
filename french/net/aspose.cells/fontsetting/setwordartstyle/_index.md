---
title: "FontSetting.SetWordArtStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FontSetting. Définit le style WordArt prédéfini"
type: docs
url: /fr/net/aspose.cells/fontsetting/setwordartstyle/
---
## FontSetting.SetWordArtStyle method

Définit le style WordArt prédéfini.

```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| style | PresetWordArtStyle | Le style WordArt prédéfini. |

### Remarques

Uniquement pour le texte de la forme/graphique.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class FontSettingMethodSetWordArtStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter du texte à la cellule A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text for WordArt");

            // Créer un paramètre de police pour le texte dans la cellule A1
            FontSetting fontSetting = new FontSetting(0, cell.StringValue.Length, workbook.Worksheets);

            try
            {
                // Appliquer le style WordArt au paramètre de police
                fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle3);

                Console.WriteLine("WordArt style applied successfully to the text.");
                
                // Afficher l'effet en enregistrant le classeur
                worksheet.AutoFitColumn(0);
                worksheet.AutoFitRow(0);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetWordArtStyle method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("FontSettingMethodSetWordArtStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


