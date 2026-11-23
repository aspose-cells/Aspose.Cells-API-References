---
title: "SettableGlobalizationSettings.SetLocalFunctionName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Définit le nom de fonction dépendant de la locale correspondant au nom de fonction standard donné"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/setlocalfunctionname/
---
## SettableGlobalizationSettings.SetLocalFunctionName method

Définit le nom de fonction dépendant de la langue correspondant au nom de fonction standard donné.

```csharp
public void SetLocalFunctionName(string standardName, string localName, bool bidirectional)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| standardName | String | Nom de fonction standard (locale en-US). |
| localName | String | Nom de fonction dépendant de la locale |
| bidirectional | Boolean | Indique si le nom de fonction local doit être mappé automatiquement au nom de fonction standard. Si vrai, le nom local sera mappé automatiquement au nom standard afin que l'utilisateur n'ait pas besoin d'appeler [`SetStandardFunctionName`](../setstandardfunctionname/) à nouveau pour la même paire de noms standard et local. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalFunctionNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des paramètres de mondialisation
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Appeler SetLocalFunctionName pour mapper le nom de fonction standard au nom local
                settings.SetLocalFunctionName("SUM", "SOMMA", true); // Italian localization for SUM function
                settings.SetLocalFunctionName("AVERAGE", "MEDIA", true); // Italian localization for AVERAGE function

                // Appliquer les paramètres au classeur
                workbook.Settings.GlobalizationSettings = settings;

                // Créer des formules en utilisant à la fois les noms standard et localisés
                worksheet.Cells["A1"].Formula = "=SUM(B1:B5)";
                worksheet.Cells["A2"].Formula = "=SOMMA(B1:B5)";
                worksheet.Cells["A3"].Formula = "=AVERAGE(B1:B5)";
                worksheet.Cells["A4"].Formula = "=MEDIA(B1:B5)";

                // Calculer les formules
                workbook.CalculateFormula();

                Console.WriteLine("SetLocalFunctionName executed successfully with parameters (String, String, Boolean)");
                Console.WriteLine("Standard and localized function names work equivalently in formulas.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalFunctionName method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("MethodSetLocalFunctionNameWithStringStringBooleanDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


