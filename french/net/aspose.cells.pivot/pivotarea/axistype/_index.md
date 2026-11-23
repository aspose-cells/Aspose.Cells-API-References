---
title: "PivotArea.AxisType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotArea. Obtient et définit la région du tableau croisé dynamique à laquelle cette règle s'applique"
type: docs
url: /fr/net/aspose.cells.pivot/pivotarea/axistype/
---
## PivotArea.AxisType property

Obtient et définit la région du PivotTable à laquelle cette règle s'applique.

```csharp
public PivotFieldType AxisType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyAxisTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["A3"].Value = "Clothing";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 800;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajoutez des champs aux zones du tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);  // Sales

            // Créer et configurer PivotArea
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row; // Demonstrate AxisType property
            pivotArea.RuleType = PivotAreaType.Normal;

            // Sélectionner la zone pivot
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            // Enregistrez le classeur
            workbook.Save("PivotAreaAxisTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


