---
title: "PivotTable.HasBlankRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique s'il faut ajouter des lignes vides. Cette propriété ne s'applique qu'aux types de format automatique du PivotTable qui nécessitent d'ajouter des lignes vides"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/hasblankrows/
---
## PivotTable.HasBlankRows property

Indique s'il faut ajouter des lignes vides. Cette propriété ne s'applique qu'aux types de format automatique du PivotTable qui nécessitent d'ajouter des lignes vides.

```csharp
[Obsolete("Use PivotField.InsertBlankRow property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBlankRows { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.InsertBlankRow. Cette méthode sera supprimée 12 mois plus tard à compter d'avril 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyHasBlankRowsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet dataSheet = wb.Worksheets[0];
            
            // Créer des données d'exemple
            dataSheet.Cells[0, 0].PutValue("Category");
            dataSheet.Cells[0, 1].PutValue("Product");
            dataSheet.Cells[0, 2].PutValue("Sales");
            
            Random rnd = new Random();
            for (int i = 1; i <= 10; i++)
            {
                dataSheet.Cells[i, 0].PutValue(rnd.Next(2) == 0 ? "Electronics" : "Furniture");
                dataSheet.Cells[i, 1].PutValue("Product " + rnd.Next(1, 4));
                dataSheet.Cells[i, 2].PutValue(rnd.Next(100, 1000));
            }

            // Ajouter un tableau croisé dynamique
            Worksheet pivotSheet = wb.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Sheet1!A1:C11", "A1", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // Configurer le tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales
            
            // Démontrer la propriété HasBlankRows
            pivotTable.HasBlankRows = false; // Remove blank lines between items
            
            // Enregistrez le classeur
            wb.Save("PivotTableHasBlankRowsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


