---
title: "GlobalizationSettings.GetDataFieldHeaderNameOfPivotTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GlobalizationSettings. Obtient le nom de l’en-tête du champ de la zone de valeurs dans le tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/
---
## GlobalizationSettings.GetDataFieldHeaderNameOfPivotTable method

Obtient le nom de l’en-tête du champ de la zone de valeurs dans le tableau croisé dynamique.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfDataFieldHeader() method instead.")]
public virtual string GetDataFieldHeaderNameOfPivotTable()
```

### Valeur de retour

Le nom de l’en-tête du champ de données

### Remarques

NOTE: Ce membre est maintenant obsol\u00e8te. \u00c0 la place, veuillez utiliser la m\u00e9thode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Cette propri\u00e9t\u00e9 sera supprim\u00e9e 12 mois plus tard \u00e0 compter de d\u00e9cembre 2022. Aspose s'excuse pour tout d\u00e9sagr\u00e9ment que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetDataFieldHeaderNameOfPivotTableDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 200;

            // Définir des paramètres de globalisation personnalisés
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Créer un tableau croisé dynamique et configurer les champs
                int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B3", "D1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category as row
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);  // Value as data

                // Actualiser le tableau croisé dynamique pour appliquer les changements de localisation
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable created with custom data field header name.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("GlobalizationSettingsMethodDemo.xlsx");
        }
    }

    // Implémentation personnalisée de GlobalizationSettings
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetDataFieldHeaderNameOfPivotTable()
        {
            return "Custom Values";
        }
    }
}
```

### Voir aussi

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


