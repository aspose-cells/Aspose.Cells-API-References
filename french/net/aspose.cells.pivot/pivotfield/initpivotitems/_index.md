---
title: "PivotField.InitPivotItems"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PivotField method. Initialise les éléments pivot du champ pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/initpivotitems/
---
## PivotField.InitPivotItems method

Initialise les éléments pivot du champ pivot

```csharp
[Obsolete("Please simply remove calling this method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void InitPivotItems()
```

### Remarques

NOTE: Cette méthode est maintenant obsolète. Veuillez simplement supprimer l'appel à cette méthode. Cette méthode sera supprimée 6 mois après octobre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodInitPivotItemsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Bike");
            worksheet.Cells["A3"].PutValue("Car");
            worksheet.Cells["A4"].PutValue("Bike");
            worksheet.Cells["A5"].PutValue("Car");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);
            worksheet.Cells["B5"].PutValue(2500);

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Obtenez le champ du tableau croisé
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Initialiser les éléments pivot
                pivotField.InitPivotItems();

                // Afficher les éléments pivot
                Console.WriteLine("Pivot Items after initialization:");
                foreach (PivotItem item in pivotField.PivotItems)
                {
                    Console.WriteLine(item.Name);
                }

                // Enregistrez le classeur
                workbook.Save("PivotFieldInitPivotItemsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InitPivotItems method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


