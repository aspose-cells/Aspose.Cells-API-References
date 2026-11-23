---
title: "GlobalizationSettings.GetTotalName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GlobalizationSettings. Obtient le nom total de la fonction"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/gettotalname/
---
## GlobalizationSettings.GetTotalName method

Obtient le nom total de la fonction.

```csharp
public virtual string GetTotalName(ConsolidationFunction functionType)
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
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B3"].Value = 2500;
            worksheet.Cells["A4"].Value = "Bike";
            worksheet.Cells["B4"].Value = 1500;

            // Créer des paramètres de mondialisation personnalisés
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Démontrer l’appel direct de la méthode
                Console.WriteLine("Sum Total Name: " + 
                    customSettings.GetTotalName(ConsolidationFunction.Sum));
                
                // Créer un tableau croisé dynamique pour déclencher l’utilisation de GetTotalName
                int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B4", "D1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                PivotField dataField = pivotTable.DataFields[dataFieldIndex];
                dataField.Function = ConsolidationFunction.Sum;

                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable created with custom total names");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsMethodGetTotalNameDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetTotalName(ConsolidationFunction functionType)
            {
                return functionType switch
                {
                    ConsolidationFunction.Sum => "[Sum Custom]",
                    ConsolidationFunction.Count => "[Count Custom]",
                    _ => base.GetTotalName(functionType)
                };
            }
        }
    }
}
```

### Voir aussi

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


