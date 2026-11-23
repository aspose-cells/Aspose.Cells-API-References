---
title: "GlobalizationSettings.GetPivotGrandTotalName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GlobalizationSettings. Obtient le nom du libellé Grand Total dans le tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/getpivotgrandtotalname/
---
## GlobalizationSettings.GetPivotGrandTotalName method

Obtient le nom du libellé "Grand Total" dans le tableau croisé dynamique.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfGrandTotal() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetPivotGrandTotalName()
```

### Valeur de retour

Le nom du libellé "Grand Total"

### Remarques

NOTE: Ce membre est maintenant obsol\u00e8te. \u00c0 la place, veuillez utiliser la m\u00e9thode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Cette propri\u00e9t\u00e9 sera supprim\u00e9e 12 mois plus tard \u00e0 compter de d\u00e9cembre 2022. Aspose s'excuse pour tout d\u00e9sagr\u00e9ment que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetPivotGrandTotalNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir des paramètres de globalisation personnalisés
            var settings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Générez des données d'exemple pour le tableau croisé dynamique
            var cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Q1";
            cells["C1"].Value = "Q2";
            cells["A2"].Value = "Electronics";
            cells["B2"].Value = 1500;
            cells["C2"].Value = 2200;
            cells["A3"].Value = "Clothing";
            cells["B3"].Value = 900;
            cells["C3"].Value = 1300;

            // Créez un tableau croisé dynamique avec plusieurs champs de données
            int pivotTableIndex = worksheet.PivotTables.Add("PivotTable", "A1:C3", "E4");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Q1
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Q2

            // Actualiser et calculer le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            try
            {
                // Démontrer l'appel de GetPivotGrandTotalName
                string grandTotalName = settings.GetPivotGrandTotalName();
                Console.WriteLine($"Custom Grand Total Name: {grandTotalName}");

                // Enregistrer le classeur modifié
                workbook.Save("GlobalizationSettingsMethodGetPivotGrandTotalNameDemo.xlsx");
                Console.WriteLine("Spreadsheet saved. Check output file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetPivotGrandTotalName()
            {
                return "[Custom Grand Total]";
            }
        }
    }
}
```

### Voir aussi

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


