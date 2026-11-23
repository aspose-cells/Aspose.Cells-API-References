---
title: "GlobalizationSettings.GetAllName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "M\\u00e9thode GlobalizationSettings. Obtient le nom de l\\u00e9tiquette All dans le tableau crois\\u00e9 dynamique"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/getallname/
---
## GlobalizationSettings.GetAllName method

Obtient le nom de l\u00e9tiquette "(All)" dans le tableau crois\u00e9 dynamique.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfAll() method instead.")]
public virtual string GetAllName()
```

### Valeur de retour

Le nom de l\u00e9tiquette "(All)"

### Remarques

NOTE: Ce membre est maintenant obsol\u00e8te. \u00c0 la place, veuillez utiliser la m\u00e9thode GlobalizationSettings.GetColumnLabelsOfPivotTable(). Cette propri\u00e9t\u00e9 sera supprim\u00e9e 12 mois plus tard \u00e0 compter de d\u00e9cembre 2022. Aspose s'excuse pour tout d\u00e9sagr\u00e9ment que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetAllNameDemo
    {
        public static void Run()
        {
            // Cr\u00e9er un nouveau classeur avec des param\u00e8tres de mondialisation personnalis\u00e9s
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            // Acc\u00e9der \u00e0 l'instance des param\u00e8tres personnalis\u00e9s
            CustomGlobalizationSettings settings = (CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings;

            try
            {
                // Appelez la méthode GetAllName et affichez le résultat
                string allName = settings.GetAllName();
                Console.WriteLine($"Custom (All) label: {allName}");

                // Créez un tableau croisé dynamique d'exemple pour démontrer l'effet de la localisation
                Worksheet worksheet = workbook.Worksheets[0];
                CreateSampleData(worksheet);
                CreatePivotTable(worksheet);

                Console.WriteLine("Demo executed successfully. Check output file's pivot table labels.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("MethodGetAllNameDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Créer des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bikes";
            worksheet.Cells["A3"].Value = "Cars";
            worksheet.Cells["A4"].Value = "Bikes";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2500;
            worksheet.Cells["B4"].Value = 1500;
        }

        private static void CreatePivotTable(Worksheet worksheet)
        {
            // Créez un tableau croisé dynamique en utilisant des données d'exemple
            int pivotIndex = worksheet.PivotTables.Add(
                "PivotTable",
                "A1:B4",
                "E3"
            );
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Configurez la structure du tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields[0]); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields[1]); // Sales

            // Actualisez le tableau pour appliquer les paramètres de localisation
            pivotTable.RefreshData();
            pivotTable.CalculateData();
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetAllName()
        {
            // L'implémentation personnalisée renvoie le libellé "All" localisé
            return "[Custom All Selection]";
        }
    }
}
```

### Voir aussi

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


