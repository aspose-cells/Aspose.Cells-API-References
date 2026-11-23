---
title: "PivotTable.CustomListSort"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique si l’on doit prendre en compte les listes personnalisées intégrées lors du tri des données"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/customlistsort/
---
## PivotTable.CustomListSort property

Indique s’il faut prendre en compte la liste personnalisée intégrée lors du tri des données

```csharp
public bool CustomListSort { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyCustomListSortDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Pear";
            cells["B5"].Value = 5;

            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Ajouter le champ de ligne et le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Activer le tri des listes personnalisées
            pivotTable.CustomListSort = true;

            // Enregistrez le classeur
            workbook.Save("PivotTable_CustomListSort_Example.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


