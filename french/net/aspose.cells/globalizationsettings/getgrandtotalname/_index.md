---
title: "GlobalizationSettings.GetGrandTotalName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GlobalizationSettings. Obtient le nom du total général de la fonction"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/getgrandtotalname/
---
## GlobalizationSettings.GetGrandTotalName method

Obtient le nom du total général de la fonction.

```csharp
public virtual string GetGrandTotalName(ConsolidationFunction functionType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| functionType | ConsolidationFunction | Le type de fonction. |

### Valeur de retour

Le nom du total général de la fonction.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetGrandTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Générez des données d'exemple pour le tableau croisé dynamique
            CreateSampleData(worksheet);

            // Instancier des paramètres de mondialisation personnalisés
            var globalizationSettings = new CustomGlobalizationSettings();
            
            try
            {
                // Démontrer l’appel direct de la méthode
                string grandTotalName = globalizationSettings.GetGrandTotalName(ConsolidationFunction.Sum);
                Console.WriteLine($"Grand Total Name: {grandTotalName}");

                // Appliquer la personnalisation aux paramètres du classeur
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Créer un tableau croisé dynamique pour démontrer l'effet
                CreatePivotTable(worksheet);

                Console.WriteLine("Method executed successfully. Check output file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetGrandTotalName method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("GrandTotalNameDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            var cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Value";
            cells["A2"].Value = "Electronics";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Furniture";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "Electronics";
            cells["B4"].Value = 800;
        }

        private static void CreatePivotTable(Worksheet worksheet)
        {
            // Créer un tableau croisé dynamique en utilisant la plage de données d'exemple
            int pivotTableIndex = worksheet.PivotTables.Add("PivotTable", "A1:B4", "D1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Configurer les champs du tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            dataField.Function = ConsolidationFunction.Sum;

            // Actualiser le tableau pour appliquer les paramètres
            pivotTable.RefreshData();
            pivotTable.CalculateData();
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetGrandTotalName(ConsolidationFunction functionType)
        {
            // Implémentation personnalisée basée sur la fonction de consolidation
            return functionType == ConsolidationFunction.Sum 
                ? "**[Sum Total]**" 
                : base.GetGrandTotalName(functionType);
        }
    }
}
```

### Voir aussi

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


