---
title: "FontConfigs.SetFontFolders"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FontConfigs. Définit le dossier des polices"
type: docs
url: /fr/net/aspose.cells/fontconfigs/setfontfolders/
---
## FontConfigs.SetFontFolders method

Définit le dossier des polices

```csharp
public static void SetFontFolders(string[] fontFolders, bool recursive)
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

    public class FontConfigsMethodSetFontFoldersWithStringBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir du texte qui utilisera des polices personnalisées
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // Préparer les dossiers de polices (remplacer par les chemins réels sur votre système)
            string[] fontFolders = new string[] 
            {
                @"C:\Windows\Fonts",
                @"D:\CustomFonts"
            };
            bool recursiveSearch = true;

            try
            {
                // Appeler la méthode SetFontFolders avec des paramètres String[] et Boolean
                FontConfigs.SetFontFolders(fontFolders, recursiveSearch);

                // Appliquer une police qui pourrait se trouver dans l'un de ces dossiers
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "SomeCustomFont"; // Replace with actual font name
                worksheet.Cells["A1"].SetStyle(style);

                Console.WriteLine("Font folders set successfully. Workbook may use fonts from these locations.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font folders: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("FontConfigsSetFontFoldersDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


