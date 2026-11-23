---
title: "SettableGlobalizationSettings.SetStandardFunctionName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Définit le nom de fonction dépendant de la locale selon le nom de fonction standard fourni"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/setstandardfunctionname/
---
## SettableGlobalizationSettings.SetStandardFunctionName method

Définit le nom de fonction dépendant de la langue selon le nom de fonction standard donné.

```csharp
public void SetStandardFunctionName(string localName, string standardName, bool bidirectional)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| localName | String | Nom de fonction dépendant de la locale |
| standardName | String | Nom de fonction standard (locale en-US). |
| bidirectional | Boolean | Indique si le nom de fonction standard doit être automatiquement mappé au nom de fonction local. Si vrai, le nom standard sera automatiquement mappé au nom local de sorte que l'utilisateur n'ait pas besoin d'appeler [`SetLocalFunctionName`](../setlocalfunctionname/) à nouveau pour la même paire de noms standard et local |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardFunctionNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des paramètres de mondialisation personnalisés
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Appeler SetStandardFunctionName pour mapper un nom de fonction local au nom standard
                settings.SetStandardFunctionName("LOCAL_SUM", "SUM", true);

                // Appliquer les paramètres au classeur
                workbook.Settings.GlobalizationSettings = settings;

                // Créer une formule en utilisant le nom de fonction local
                worksheet.Cells["A1"].Formula = "=LOCAL_SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 10;
                worksheet.Cells["B2"].Value = 20;
                worksheet.Cells["B3"].Value = 30;

                // Calculer la formule
                workbook.CalculateFormula();

                Console.WriteLine("Formula with local function name 'LOCAL_SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardFunctionName method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("SetStandardFunctionNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


