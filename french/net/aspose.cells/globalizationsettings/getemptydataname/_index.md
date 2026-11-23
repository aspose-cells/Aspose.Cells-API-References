---
title: "GlobalizationSettings.GetEmptyDataName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GlobalizationSettings. Obtient le nom de l'étiquette vide dans le tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/getemptydataname/
---
## GlobalizationSettings.GetEmptyDataName method

Obtient le nom de l'étiquette "(blank)" dans le tableau croisé dynamique.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfEmptyData() method instead.")]
public virtual string GetEmptyDataName()
```

### Valeur de retour

Le nom des données vides

### Remarques

NOTE: Ce membre est maintenant obsol\u00e8te. \u00c0 la place, veuillez utiliser la m\u00e9thode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Cette propri\u00e9t\u00e9 sera supprim\u00e9e 12 mois plus tard \u00e0 compter de d\u00e9cembre 2022. Aspose s'excuse pour tout d\u00e9sagr\u00e9ment que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetEmptyDataNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple avec des cellules vides
            object[,] data = new object[,]
            {
                {"Category", "Sales"},
                {"Electronics", 1500},
                {null, 2000}, // Empty category cell
                {"Furniture", 3000}
            };

            // Remplir la feuille de calcul
            int rows = data.GetLength(0);
            int cols = data.GetLength(1);
            for (int i = 0; i < rows; i++)
            {
                for (int j = 0; j < cols; j++)
                {
                    worksheet.Cells[i, j].PutValue(data[i, j]);
                }
            }

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            // Corrigé : Supprimer l'affectation invalide du résultat de AddFieldToArea
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Configurer les paramètres de mondialisation personnalisés
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Actualiser le tableau croisé dynamique pour appliquer la localisation
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Démontrer l’appel direct de la méthode
                string emptyName = workbook.Settings.GlobalizationSettings.GetEmptyDataName();
                Console.WriteLine($"Custom empty data label: {emptyName}");

                workbook.Save("GlobalizationGetEmptyDataNameDemo.xlsx");
                Console.WriteLine("Demo executed successfully. Check output file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            [Obsolete]
            public override string GetEmptyDataName()
            {
                return "[[UNSPECIFIED]]"; // Custom empty data label
            }
        }
    }
}
```

### Voir aussi

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


