---
title: "PivotField.ClearFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotField. Supprime le paramètre de filtre sur ce champ pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/clearfilter/
---
## PivotField.ClearFilter method

Efface le paramètre de filtre sur ce champ pivot.

```csharp
public void ClearFilter()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodClearFilterDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["A4"].Value = "Fruit";
            worksheet.Cells["A5"].Value = "Vegetable";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;
            worksheet.Cells["B5"].Value = 300;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Obtenez le champ du tableau croisé
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Appliquez d'abord un filtre pour démontrer sa suppression
                pivotField.FilterByLabel(PivotFilterType.CaptionEqual, "Fruit", null);

                // Appelez la méthode ClearFilter
                pivotField.ClearFilter();

                Console.WriteLine("ClearFilter method executed successfully");
                Console.WriteLine("All filters have been removed from the pivot field");

                // Actualisez le tableau croisé dynamique pour afficher les modifications
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFilter method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("PivotFieldMethodClearFilterDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


