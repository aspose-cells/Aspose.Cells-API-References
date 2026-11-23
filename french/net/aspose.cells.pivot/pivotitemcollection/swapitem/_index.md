---
title: "PivotItemCollection.SwapItem"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotItemCollection. Échange directement deux éléments"
type: docs
url: /fr/net/aspose.cells.pivot/pivotitemcollection/swapitem/
---
## PivotItemCollection.SwapItem method

Échange directement deux éléments.

```csharp
public void SwapItem(int index1, int index2)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| index1 | Int32 |  |
| index2 | Int32 |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemCollectionMethodSwapItemWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Obtenir les éléments du tableau croisé dynamique
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            try
            {
                // Afficher l'ordre original
                Console.WriteLine("Original order:");
                foreach (PivotItem item in pivotItems)
                {
                    Console.WriteLine(item.Name);
                }

                // Échanger les éléments aux indices 0 et 1
                pivotItems.SwapItem(0, 1);

                // Afficher le nouvel ordre
                Console.WriteLine("\nAfter swapping:");
                foreach (PivotItem item in pivotItems)
                {
                    Console.WriteLine(item.Name);
                }

                Console.WriteLine("SwapItem method executed successfully with parameters (0, 1)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SwapItem method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("PivotItemCollectionMethodSwapItemWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


