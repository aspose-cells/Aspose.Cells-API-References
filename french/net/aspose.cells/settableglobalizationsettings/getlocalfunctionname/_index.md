---
title: "SettableGlobalizationSettings.GetLocalFunctionName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Obtient le nom de fonction dépendant de la locale selon le nom de fonction standard fourni"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/getlocalfunctionname/
---
## SettableGlobalizationSettings.GetLocalFunctionName method

Obtient le nom de fonction dépendant de la langue selon le nom de fonction standard fourni.

```csharp
public override string GetLocalFunctionName(string standardName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| standardName | String | Nom de fonction standard (locale en-US). |

### Valeur de retour

Nom de fonction dépendant de la locale. La locale a été spécifiée par le classeur pour lequel ces paramètres sont utilisés.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des paramètres de mondialisation personnalisés
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Définir un nom de fonction local personnalisé pour "SUM"
            settings.SetLocalFunctionName("SUM", "SOMME", true);

            // Appliquer les paramètres au classeur
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Appeler GetLocalFunctionName pour récupérer le nom localisé
                string localName = settings.GetLocalFunctionName("SUM");
                
                // Afficher le résultat
                Console.WriteLine($"Localized function name for 'SUM': {localName}");

                // Utiliser la fonction localisée dans une cellule
                worksheet.Cells["A1"].Formula = "=SOMME(B1:B5)";
                worksheet.Cells["B1"].PutValue(1);
                worksheet.Cells["B2"].PutValue(2);
                worksheet.Cells["B3"].PutValue(3);
                worksheet.Cells["B4"].PutValue(4);
                worksheet.Cells["B5"].PutValue(5);

                // Calculer les formules
                workbook.CalculateFormula();

                // Afficher le résultat
                Console.WriteLine($"Calculation result with localized function: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalFunctionName method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("MethodGetLocalFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


