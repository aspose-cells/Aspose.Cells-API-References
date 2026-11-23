---
title: "PivotTable.ShowColumnGrandTotals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique s’il faut afficher les totaux généraux pour les colonnes de ce tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/showcolumngrandtotals/
---
## PivotTable.ShowColumnGrandTotals property

Indique s'il faut afficher les totaux généraux pour les colonnes de ce tableau croisé dynamique.

```csharp
public bool ShowColumnGrandTotals { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowColumnGrandTotalsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["A5"].Value = "Apple";
            cells["B2"].Value = 5;
            cells["B3"].Value = 3;
            cells["B4"].Value = 6;
            cells["B5"].Value = 2;

            // Ajouter un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Configurer le tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit as rows
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sum of Quantity

            // Démontrer la propriété ShowColumnGrandTotals
            pivotTable.ShowColumnGrandTotals = false; // Disable column grand totals
            Console.WriteLine("Column Grand Totals Visible: " + pivotTable.ShowColumnGrandTotals);

            // Enregistrez le classeur
            workbook.Save("PivotTableShowColumnGrandTotalsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


