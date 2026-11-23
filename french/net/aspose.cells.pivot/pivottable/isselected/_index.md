---
title: "PivotTable.IsSelected"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PivotTable property. Indique si ce tableau croisé dynamique est sélectionné"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/isselected/
---
## PivotTable.IsSelected property

Indique si ce tableau croisé dynamique est sélectionné.

```csharp
public bool IsSelected { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsSelectedDemo
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
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Ajouter un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];

            // Initialement, IsSelected est false
            Console.WriteLine("PivotTable IsSelected initially: " + pivotTable.IsSelected);

            // Sélectionnez le tableau croisé dynamique
            pivotTable.IsSelected = true;
            Console.WriteLine("PivotTable IsSelected after setting to true: " + pivotTable.IsSelected);

            // Désélectionnez le tableau croisé dynamique
            pivotTable.IsSelected = false;
            Console.WriteLine("PivotTable IsSelected after setting to false: " + pivotTable.IsSelected);
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


