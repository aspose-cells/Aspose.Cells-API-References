---
title: "PivotShowValuesSetting.BaseFieldIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotShowValuesSetting. Représente le champ de base pour un calcul ShowDataAs lorsque le calcul ShowDataAs est utilisé"
type: docs
url: /fr/net/aspose.cells.pivot/pivotshowvaluessetting/basefieldindex/
---
## PivotShowValuesSetting.BaseFieldIndex property

Représente le champ de base pour un calcul ShowDataAs lorsque le calcul ShowDataAs est utilisé.

```csharp
public int BaseFieldIndex { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotShowValuesSettingPropertyBaseFieldIndexDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 200;

            try
            {
                // Créer un tableau croisé dynamique
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Ajouter des champs au tableau croisé dynamique
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Obtenir le champ de données et son paramètre d'affichage des valeurs
                PivotField dataField = pivotTable.DataFields[0];
                PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

                // Définir le type de calcul pour démontrer l'utilisation de BaseFieldIndex
                showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOf;

                // Définir et obtenir la propriété BaseFieldIndex
                showValuesSetting.BaseFieldIndex = 0;
                Console.WriteLine("BaseFieldIndex value: " + showValuesSetting.BaseFieldIndex);

                // Actualiser et calculer le tableau croisé dynamique
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Enregistrez le classeur
                workbook.Save("BaseFieldIndexDemo.xlsx");
                Console.WriteLine("BaseFieldIndex has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


