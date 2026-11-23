---
title: "SettableGlobalizationSettings.GetStandardFunctionName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Obtient le nom de fonction standard en fonction du nom de fonction dépendant de la locale fourni"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/getstandardfunctionname/
---
## SettableGlobalizationSettings.GetStandardFunctionName method

Obtient le nom de fonction standard selon le nom de fonction dépendant de la langue fourni.

```csharp
public override string GetStandardFunctionName(string localName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| localName | String | Nom de fonction dépendant de la locale. La locale a été spécifiée par le classeur pour lequel ces paramètres sont utilisés. |

### Valeur de retour

Nom de fonction standard (locale en-US).

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des paramètres de mondialisation personnalisés
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Définir une correspondance de nom de fonction locale
            settings.SetStandardFunctionName("LocalSum", "SUM", true);

            // Appliquer les paramètres au classeur
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Appeler GetStandardFunctionName avec un nom de fonction local
                string standardName = settings.GetStandardFunctionName("LocalSum");
                
                // Afficher le résultat
                Console.WriteLine($"Standard function name for 'LocalSum' is: {standardName}");

                // Utiliser la fonction standard dans une formule de cellule
                worksheet.Cells["A1"].Formula = $"={standardName}(1,2,3)";
                worksheet.Cells["A2"].Value = 1;
                worksheet.Cells["A3"].Value = 2;
                worksheet.Cells["A4"].Value = 3;

                // Calculer la formule
                workbook.CalculateFormula();

                // Afficher le résultat
                Console.WriteLine($"Formula result in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


