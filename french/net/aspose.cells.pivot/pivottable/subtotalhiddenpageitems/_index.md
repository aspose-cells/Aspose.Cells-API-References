---
title: "PivotTable.SubtotalHiddenPageItems"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique si les éléments de champ de page masqués dans le rapport PivotTable sont inclus dans les sous‑totaux de lignes et de colonnes, les totaux de bloc et les totaux généraux. La valeur par défaut est False"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/subtotalhiddenpageitems/
---
## PivotTable.SubtotalHiddenPageItems property

Indique si les éléments de champ de page masqués dans le rapport PivotTable sont inclus dans les sous‑totaux de lignes et de colonnes, les totaux de blocs et les totaux généraux. La valeur par défaut est False.

```csharp
public bool SubtotalHiddenPageItems { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertySubtotalHiddenPageItemsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Apple";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Orange";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            
            cells["A4"].Value = "Banana";
            cells["B4"].Value = "North";
            cells["C4"].Value = 1500;
            
            cells["A5"].Value = "Apple";
            cells["B5"].Value = "South";
            cells["C5"].Value = 1200;

            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Ajouter des champs
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Définir la propriété SubtotalHiddenPageItems
            pivotTable.SubtotalHiddenPageItems = true;
            Console.WriteLine("SubtotalHiddenPageItems set to: " + pivotTable.SubtotalHiddenPageItems);

            // Actualiser et calculer les données
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotTable_SubtotalHiddenPageItemsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


