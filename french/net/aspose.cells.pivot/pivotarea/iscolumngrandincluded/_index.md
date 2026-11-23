---
title: "PivotArea.IsColumnGrandIncluded"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotArea. Indique si le total général de la colonne est inclus"
type: docs
url: /fr/net/aspose.cells.pivot/pivotarea/iscolumngrandincluded/
---
## PivotArea.IsColumnGrandIncluded property

Indique si le total général de la colonne est inclus.

```csharp
public bool IsColumnGrandIncluded { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyIsColumnGrandIncludedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Données d'exemple
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter des champs
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Configurer la zone pivot
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.IsColumnGrandIncluded = true; // Demonstrate property usage
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.RuleType = PivotAreaType.Normal;

            // Enregistrez le classeur
            workbook.Save("PivotAreaIsColumnGrandIncludedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


