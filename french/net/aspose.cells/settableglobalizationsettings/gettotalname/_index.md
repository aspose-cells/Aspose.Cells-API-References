---
title: "SettableGlobalizationSettings.GetTotalName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Obtient le nom total d'une fonction spécifique"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/gettotalname/
---
## SettableGlobalizationSettings.GetTotalName method

Obtient le nom total de la fonction spécifique.

```csharp
public override string GetTotalName(ConsolidationFunction functionType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| functionType | ConsolidationFunction | Le type de fonction. |

### Valeur de retour

Le nom total de la fonction.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez une instance de SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Appeler GetTotalName avec ConsolidationFunction.Sum
                string totalName = globalizationSettings.GetTotalName(ConsolidationFunction.Sum);
                
                // Afficher le résultat
                Console.WriteLine($"Total name for Sum function: {totalName}");

                // Ajouter des données pour démontrer l'effet (bien que GetTotalName ne modifie pas la feuille de calcul)
                worksheet.Cells["A1"].PutValue("Values");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["B1"].PutValue("Total");
                worksheet.Cells["B4"].Formula = "=SUM(A2:A4)";
                
                // Calculer les formules
                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTotalName method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("SettableGlobalizationSettingsMethodGetTotalNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


