---
title: "IndividualFontConfigs.SetFontFolders"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode IndividualFontConfigs. Définit les dossiers de polices"
type: docs
url: /fr/net/aspose.cells/individualfontconfigs/setfontfolders/
---
## IndividualFontConfigs.SetFontFolders method

Définit les dossiers de police

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fontFolders | String[] | Les dossiers qui contiennent les polices TrueType. |
| recursive | Boolean | Détermine s'il faut ou non analyser les sous-dossiers. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodSetFontFoldersWithStringBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une instance de IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Préparer le tableau des dossiers de polices
            string[] fontFolders = new string[] { @"C:\Windows\Fonts", @"D:\CustomFonts" };
            bool recursiveSearch = true;

            try
            {
                // Appeler la méthode SetFontFolders avec des paramètres String[] et Boolean
                fontConfigs.SetFontFolders(fontFolders, recursiveSearch);

                // Démontrer l'effet en utilisant une police personnalisée
                worksheet.Cells["A1"].PutValue("Text with custom font");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "SomeCustomFont"; // Assuming this font exists in one of the folders
                worksheet.Cells["A1"].SetStyle(style);

                Console.WriteLine("SetFontFolders method executed successfully with parameters (String[], Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontFolders method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("SetFontFoldersDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


