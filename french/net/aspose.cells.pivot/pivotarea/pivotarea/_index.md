---
title: "PivotArea.PivotArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur PivotArea. Présente la zone sélectionnée du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivotarea/pivotarea/
---
## PivotArea constructor

Présente la zone sélectionnée du PivotTable.

```csharp
public PivotArea(PivotTable table)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| table | PivotTable |  |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaMethodctorWithPivotTableDemo
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
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Démontrer le constructeur PivotArea avec le paramètre PivotTable
            PivotArea pivotArea = new PivotArea(pivotTable);
            
            // Configurer la zone pivot
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            
            // Enregistrez le classeur
            workbook.Save("PivotAreaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../../pivottable/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


