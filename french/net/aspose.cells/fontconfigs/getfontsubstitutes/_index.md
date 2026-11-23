---
title: "FontConfigs.GetFontSubstitutes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FontConfigs. Retourne un tableau contenant les noms de substituts de police à utiliser si la police d'origine n'est pas présente"
type: docs
url: /fr/net/aspose.cells/fontconfigs/getfontsubstitutes/
---
## FontConfigs.GetFontSubstitutes method

Renvoie un tableau contenant les noms de substituts de police à utiliser si la police d'origine n'est pas présente.

```csharp
public static string[] GetFontSubstitutes(string originalFontName)
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

    public class FontConfigsMethodGetFontSubstitutesWithStringDemo
    {
        public static void Run()
        {
            // Initialiser FontConfigs
            FontConfigs fontConfigs = new FontConfigs();

            try
            {
                // Appeler GetFontSubstitutes avec un nom de police
                string originalFontName = "Arial";
                string[] substitutes = FontConfigs.GetFontSubstitutes(originalFontName);

                // Affichez les résultats
                Console.WriteLine($"Substitute fonts for '{originalFontName}':");
                if (substitutes != null && substitutes.Length > 0)
                {
                    foreach (string substitute in substitutes)
                    {
                        Console.WriteLine(substitute);
                    }
                }
                else
                {
                    Console.WriteLine("No substitutes found for the specified font.");
                }

                // Démontrer la définition des substituts et leur récupération
                string[] newSubstitutes = new string[] { "Liberation Sans", "DejaVu Sans" };
                FontConfigs.SetFontSubstitutes(originalFontName, newSubstitutes);

                // Récupérer à nouveau les substituts pour vérifier
                substitutes = FontConfigs.GetFontSubstitutes(originalFontName);
                Console.WriteLine("\nAfter setting substitutes:");
                foreach (string substitute in substitutes)
                {
                    Console.WriteLine(substitute);
                }
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

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


