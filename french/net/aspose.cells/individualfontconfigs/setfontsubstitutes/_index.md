---
title: "IndividualFontConfigs.SetFontSubstitutes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode IndividualFontConfigs. Définit les noms de substitution de police pour un nom de police original donné"
type: docs
url: /fr/net/aspose.cells/individualfontconfigs/setfontsubstitutes/
---
## IndividualFontConfigs.SetFontSubstitutes method

Définit les noms de substituts de police pour un nom de police d'origine donné.

```csharp
public void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| originalFontName | String | Nom de police original. |
| substituteFontNames | String[] | Liste des noms de substituts de police à utiliser si la police originale n'est pas présentée. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodSetFontSubstitutesWithStringStringDemo
    {
        public static void Run()
        {
            // Créer une instance de IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Nom de police original et ses substituts
            string originalFont = "Arial";
            string[] substitutes = new string[] { "Helvetica", "Verdana", "Times New Roman" };

            try
            {
                // Appeler SetFontSubstitutes avec les paramètres spécifiés
                fontConfigs.SetFontSubstitutes(originalFont, substitutes);

                Console.WriteLine($"Successfully set font substitutes for '{originalFont}'");
                Console.WriteLine("Substitutes are:");
                foreach (var sub in substitutes)
                {
                    Console.WriteLine($"- {sub}");
                }

                // Créer un classeur pour démontrer l'effet
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Définir le style avec la police originale
                Style style = workbook.CreateStyle();
                style.Font.Name = originalFont;
                style.Font.Size = 14;
                
                worksheet.Cells["A1"].Value = "This text uses " + originalFont;
                worksheet.Cells["A1"].SetStyle(style);

                // Enregistrez le classeur
                workbook.Save("FontSubstitutesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font substitutes: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


