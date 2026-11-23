---
title: "PivotArea.IsOutline"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotArea. Indique si la règle fait référence à une zone en mode plan"
type: docs
url: /fr/net/aspose.cells.pivot/pivotarea/isoutline/
---
## PivotArea.IsOutline property

Indique si la règle se réfère à une zone en mode plan.

```csharp
public bool IsOutline { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyIsOutlineDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Créer et configurer PivotArea
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.IsOutline = false; // Disable outline style
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);

            // Enregistrez le classeur
            workbook.Save("PivotAreaIsOutlineDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


