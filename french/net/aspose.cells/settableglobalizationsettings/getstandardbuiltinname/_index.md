---
title: "SettableGlobalizationSettings.GetStandardBuiltInName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Obtient le texte standard du nom intégré selon le texte dépendant de la locale fourni"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/getstandardbuiltinname/
---
## SettableGlobalizationSettings.GetStandardBuiltInName method

Obtient le texte standard du nom intégré selon le texte dépendant de la langue fourni.

```csharp
public override string GetStandardBuiltInName(string localName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| localName | String | Texte dépendant de la locale du nom intégré. La locale a été spécifiée par le Workbook pour lequel ces paramètres sont utilisés. |

### Valeur de retour

Texte standard (locale en-US).

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez une instance de SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            // Définir un nom intégré local à des fins de démonstration
            globalizationSettings.SetLocalBuiltInName("SUM", "LocalSumName", true);

            try
            {
                // Appeler la méthode GetStandardBuiltInName avec un nom local
                string standardName = globalizationSettings.GetStandardBuiltInName("LocalSumName");
                
                // Afficher le résultat
                Console.WriteLine($"Standard name for 'LocalSumName' is: {standardName}");

                // Appliquer le résultat à une cellule
                worksheet.Cells["A1"].Formula = "=" + standardName + "(1,2,3)";
                workbook.CalculateFormula();

                // Afficher le résultat calculé
                Console.WriteLine($"Result of formula in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardBuiltInName method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


