---
title: "GlobalizationSettings.GetRowLabelsNameOfPivotTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GlobalizationSettings. Obtient le nom de l'étiquette Row Labels dans le tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/
---
## GlobalizationSettings.GetRowLabelsNameOfPivotTable method

Obtient le nom de l'étiquette "Row Labels" dans le tableau croisé dynamique.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfRowLabels() method instead.")]
public virtual string GetRowLabelsNameOfPivotTable()
```

### Valeur de retour

Le nom des étiquettes de lignes

### Remarques

NOTE: Ce membre est maintenant obsol\u00e8te. \u00c0 la place, veuillez utiliser la m\u00e9thode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Cette propri\u00e9t\u00e9 sera supprim\u00e9e 12 mois plus tard \u00e0 compter de d\u00e9cembre 2022. Aspose s'excuse pour tout d\u00e9sagr\u00e9ment que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetRowLabelsNameOfPivotTable()
        {
            return "Custom Row Labels";
        }
    }

    public class GlobalizationSettingsMethodGetRowLabelsNameOfPivotTableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple pour le tableau croisé dynamique
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["A2"].PutValue("Bikes");
            cells["A3"].PutValue("Cars");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(1000);
            cells["B3"].PutValue(2500);

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B3", "E3", "SalesPivot");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row field

            // Appliquer des paramètres de mondialisation personnalisés
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                pivotTable.RefreshData();
                pivotTable.CalculateData();
                Console.WriteLine("Pivot table created with custom row labels name.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRowLabelsNameOfPivotTable: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsMethodGetRowLabelsNameOfPivotTableDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


