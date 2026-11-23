---
title: "PivotTable.EnableFieldList"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique si la liste de champs pour le PivotTable est disponible dans la vue d'Excel"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/enablefieldlist/
---
## PivotTable.EnableFieldList property

Indique si la liste des champs du tableau croisé dynamique est disponible dans la vue d'Excel.

```csharp
public bool EnableFieldList { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyEnableFieldListDemo
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
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Définir la propriété EnableFieldList
            pivotTable.EnableFieldList = false;

            // Enregistrez le classeur
            workbook.Save("PivotTable_EnableFieldList_Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


