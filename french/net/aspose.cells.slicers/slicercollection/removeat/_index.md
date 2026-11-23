---
title: "SlicerCollection.RemoveAt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SlicerCollection. Supprime le Slicer à l'indice spécifié"
type: docs
url: /fr/net/aspose.cells.slicers/slicercollection/removeat/
---
## SlicerCollection.RemoveAt method

Supprime le Slicer à l'indice spécifié

```csharp
public void RemoveAt(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'indice de position dans la collection Slicer |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul
            Worksheet worksheet = workbook.Worksheets.Add("Sheet1");
            
            // Ajoutez des données pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Ajouter un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Ajouter des segments
            Aspose.Cells.Slicers.SlicerCollection slicers = worksheet.Slicers;
            slicers.Add(pivotTable, "Fruit", "FruitSlicer1");
            slicers.Add(pivotTable, "Fruit", "FruitSlicer2");

            // Supprimer le deuxième segment à l'index 1
            slicers.RemoveAt(1);
            
            // Enregistrez le classeur
            workbook.Save("SlicerCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


