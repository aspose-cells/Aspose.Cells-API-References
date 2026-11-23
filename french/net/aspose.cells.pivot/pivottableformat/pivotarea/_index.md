---
title: "PivotTableFormat.PivotArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTableFormat. Obtient la zone pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivottableformat/pivotarea/
---
## PivotTableFormat.PivotArea property

Obtient la zone du pivot.

```csharp
public PivotArea PivotArea { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableFormatPropertyPivotAreaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);

            // Créer un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Ajoutez des champs aux zones du tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Obtenez le format pivot et configurez sa zone pivot
            int formatIndex = pivotTable.PivotFormats.Add();
            PivotTableFormat pivotFormat = pivotTable.PivotFormats[formatIndex];
            PivotArea pivotArea = pivotFormat.PivotArea;
            
            // Définissez les propriétés de la zone pivot
            pivotArea.AxisType = PivotFieldType.Data;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;

            // Créez et appliquez le style à la zone pivot
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            pivotFormat.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("PivotTableWithPivotArea.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotArea](../../pivotarea/)
* class [PivotTableFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


