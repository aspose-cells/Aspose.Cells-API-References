---
title: "IndividualFontConfigs.GetFontSubstitutes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode IndividualFontConfigs. Retourne un tableau contenant les noms de substituts de police à utiliser si la police d'origine n'est pas présentée"
type: docs
url: /fr/net/aspose.cells/individualfontconfigs/getfontsubstitutes/
---
## IndividualFontConfigs.GetFontSubstitutes method

Renvoie un tableau contenant les noms de substituts de police à utiliser si la police d'origine n'est pas présentée.

```csharp
public string[] GetFontSubstitutes(string originalFontName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| originalFontName | String | originalFontName |

### Valeur de retour

Un tableau contenant les noms de substituts de police à utiliser si la police d'origine n'est pas présentée.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodGetFontSubstitutesWithStringDemo
    {
        public static void Run()
        {
            // Créer des configurations de police individuelles
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Définir les substituts de police pour "Arial"
            fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Calibri" });

            try
            {
                // Obtenir les substituts de police pour "Arial"
                string[] substitutes = fontConfigs.GetFontSubstitutes("Arial");

                Console.WriteLine("Font substitutes for Arial:");
                foreach (string font in substitutes)
                {
                    Console.WriteLine(font);
                }

                // Créer un classeur pour démontrer l'effet
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Définir le style avec la police originale
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].Value = "This text uses Arial font which may be substituted";

                // Enregistrez le classeur
                workbook.Save("FontSubstitutesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontSubstitutes method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


