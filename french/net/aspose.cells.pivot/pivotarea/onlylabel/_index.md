---
title: "PivotArea.OnlyLabel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotArea. Indique si seules les étiquettes de données pour une sélection d'éléments sont sélectionnées"
type: docs
url: /fr/net/aspose.cells.pivot/pivotarea/onlylabel/
---
## PivotArea.OnlyLabel property

Indique si seules les étiquettes de données d’une sélection d’éléments sont sélectionnées.

```csharp
public bool OnlyLabel { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyOnlyLabelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter des champs
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Configurer la zone pivot
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.OnlyLabel = true; // Key property demonstration
            
            // Appliquer la sélection
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            workbook.Save("PivotAreaOnlyLabelDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


