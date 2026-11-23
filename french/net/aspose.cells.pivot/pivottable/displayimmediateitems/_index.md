---
title: "PivotTable.DisplayImmediateItems"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique si les éléments des zones de lignes et de colonnes sont visibles lorsque la zone de données du PivotTable est vide. La valeur par défaut est vraie."
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/displayimmediateitems/
---
## PivotTable.DisplayImmediateItems property

Indique si les éléments des zones de lignes et de colonnes sont visibles lorsque la zone de données du PivotTable est vide. La valeur par défaut est true.

```csharp
public bool DisplayImmediateItems { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDisplayImmediateItemsDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Créer un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Démontrer la propriété DisplayImmediateItems
            Console.WriteLine("Initial DisplayImmediateItems value: " + pivotTable.DisplayImmediateItems);
            
            // Modifier la valeur de la propriété
            pivotTable.DisplayImmediateItems = false;
            Console.WriteLine("After setting to false: " + pivotTable.DisplayImmediateItems);

            // Enregistrez le classeur
            workbook.Save("PivotTableDisplayImmediateItemsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


