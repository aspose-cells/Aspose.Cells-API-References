---
title: "PivotArea.IsRowGrandIncluded"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotArea. Indique si le total général des lignes est inclus"
type: docs
url: /fr/net/aspose.cells.pivot/pivotarea/isrowgrandincluded/
---
## PivotArea.IsRowGrandIncluded property

Indique si le total général de la ligne est inclus.

```csharp
public bool IsRowGrandIncluded { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyIsRowGrandIncludedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Données d'exemple
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);

            // Créer un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Ajouter des champs
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Créer un format pivot
            int formatIndex = pivotTable.PivotFormats.Add();
            PivotTableFormat pivotFormat = pivotTable.PivotFormats[formatIndex];
            PivotArea pivotArea = pivotFormat.PivotArea;
            
            // Démontrer la propriété IsRowGrandIncluded
            pivotArea.AxisType = PivotFieldType.Data;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = false;

            // Appliquer un style pour mettre en évidence la ligne totale
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGreen;
            style.Pattern = BackgroundType.Solid;
            pivotFormat.SetStyle(style);

            workbook.Save("PivotAreaIsRowGrandIncludedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


