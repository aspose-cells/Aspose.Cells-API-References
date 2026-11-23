---
title: "FontConfigs.SetFontSubstitutes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FontConfigs. Noms de substituts de police pour le nom de police original donné"
type: docs
url: /fr/net/aspose.cells/fontconfigs/setfontsubstitutes/
---
## FontConfigs.SetFontSubstitutes method

Noms de substituts de police pour le nom de police d'origine donné.

```csharp
public static void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
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

    public class FontConfigsMethodSetFontSubstitutesWithStringStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Nom de police original qui pourrait ne pas être disponible
            string originalFontName = "Arial";
            
            // Noms de substituts de police à utiliser lorsque l'original n'est pas disponible
            string[] substituteFontNames = new string[] { "Liberation Sans", "Helvetica", "Verdana" };
            
            try
            {
                // Appeler la méthode SetFontSubstitutes pour configurer les substitutions de police
                FontConfigs.SetFontSubstitutes(originalFontName, substituteFontNames);
                
                Console.WriteLine($"Font substitutes set successfully for '{originalFontName}'");
                
                // Vérifier les substituts en les récupérant
                string[] retrievedSubstitutes = FontConfigs.GetFontSubstitutes(originalFontName);
                Console.WriteLine("Current substitutes for '{0}':", originalFontName);
                foreach (string font in retrievedSubstitutes)
                {
                    Console.WriteLine("- " + font);
                }
                
                // Appliquer la police à une cellule pour démontrer la substitution
                worksheet.Cells["A1"].PutValue("Text with potential font substitution");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = originalFontName;
                worksheet.Cells["A1"].SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontSubstitutes method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("FontSubstitutionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


