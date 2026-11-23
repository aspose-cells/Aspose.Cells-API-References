---
title: "IndividualFontConfigs.SetFontFolder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode IndividualFontConfigs. Définit le dossier des polices"
type: docs
url: /fr/net/aspose.cells/individualfontconfigs/setfontfolder/
---
## IndividualFontConfigs.SetFontFolder method

Définit le dossier des polices

```csharp
public void SetFontFolder(string fontFolder, bool recursive)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fontFolder | String | Le dossier qui contient les polices TrueType. |
| recursive | Boolean | Détermine s'il faut ou non analyser les sous-dossiers. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodSetFontFolderWithStringBooleanDemo
    {
        public static void Run()
        {
            // Créer une instance de IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();
            
            // Spécifier le chemin du dossier de polices et si la recherche doit être récursive
            string fontFolderPath = @"C:\Windows\Fonts";
            bool recursiveSearch = true;

            try
            {
                // Appeler SetFontFolder avec les paramètres spécifiés
                fontConfigs.SetFontFolder(fontFolderPath, recursiveSearch);
                
                Console.WriteLine($"Successfully set font folder to: {fontFolderPath}");
                Console.WriteLine($"Recursive search enabled: {recursiveSearch}");

                // Créer un classeur pour démontrer l'utilisation des polices
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Définir un style qui pourrait utiliser des polices du dossier spécifié
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial"; // Assuming Arial exists in the font folder
                style.Font.Size = 12;
                
                worksheet.Cells["A1"].Value = "Text with font from specified folder";
                worksheet.Cells["A1"].SetStyle(style);
                
                // Enregistrez le classeur
                workbook.Save("FontConfigDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font folder: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


