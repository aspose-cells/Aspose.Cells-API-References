---
title: "SettableGlobalizationSettings.SetTotalName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Définit le nom total d'une fonction spécifique"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/settotalname/
---
## SettableGlobalizationSettings.SetTotalName method

Définit le nom total de la fonction spécifique.

```csharp
public void SetTotalName(ConsolidationFunction functionType, string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| functionType | ConsolidationFunction | Le type de fonction. |
| name | String | Le nom total de la fonction. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettableGlobalizationSettingsMethodSetTotalNameWithConsolidationFunctionStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple pour la consolidation
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["A4"].PutValue("Total");

            // Créer des paramètres de mondialisation personnalisés
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Définir un nom total personnalisé pour la fonction Sum
                settings.SetTotalName(ConsolidationFunction.Sum, "Custom Sum Total");
                
                // Définir un nom total personnalisé pour la fonction Average
                settings.SetTotalName(ConsolidationFunction.Average, "Custom Average Total");

                // Appliquer les paramètres au classeur
                workbook.Settings.GlobalizationSettings = settings;

                // Vérifier les paramètres en récupérant les valeurs
                string sumTotalName = settings.GetTotalName(ConsolidationFunction.Sum);
                string avgTotalName = settings.GetTotalName(ConsolidationFunction.Average);

                Console.WriteLine($"Sum total name set to: {sumTotalName}");
                Console.WriteLine($"Average total name set to: {avgTotalName}");

                // Créer un tableau croisé dynamique pour démontrer l'effet
                worksheet.Cells["D1"].PutValue("Pivot Table");
                var pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
                var pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
                pivotTable.DataFields[1].Function = ConsolidationFunction.Average;
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Enregistrez le classeur
                workbook.Save("SetTotalNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTotalName method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


