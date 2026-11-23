---
title: "PivotFieldCollection.Move"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotFieldCollection. Déplace le PivotField de la position actuelle à la position de destination"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfieldcollection/move/
---
## PivotFieldCollection.Move method

Déplace le PivotField de la position actuelle vers la position de destination

```csharp
public void Move(int currPos, int destPos)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| currPos | Int32 | Position actuelle du PivotField basée sur zéro |
| destPos | Int32 | Position de destination du PivotField basée sur zéro |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionMethodMoveWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Créer des données d'exemple
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 20;

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Ajouter des champs à la zone de lignes
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1);
            
            Console.WriteLine("Before move:");
            for (int i = 0; i < pivotTable.RowFields.Count; i++)
            {
                Console.WriteLine($"Field {i}: {pivotTable.RowFields[i].Name}");
            }
            
            // Déplacez le premier champ à la position 1
            pivotTable.RowFields.Move(0, 1);
            
            Console.WriteLine("\nAfter move:");
            for (int i = 0; i < pivotTable.RowFields.Count; i++)
            {
                Console.WriteLine($"Field {i}: {pivotTable.RowFields[i].Name}");
            }
        }
    }
}
```

### Voir aussi

* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


