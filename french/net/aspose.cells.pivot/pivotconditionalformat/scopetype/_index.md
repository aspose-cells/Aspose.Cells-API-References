---
title: "PivotConditionalFormat.ScopeType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotConditionalFormat. Obtenez et définissez le type de portée pour le format conditionnel du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivotconditionalformat/scopetype/
---
## PivotConditionalFormat.ScopeType property

Obtenez et définissez le type de portée du format conditionnel du tableau croisé dynamique.

```csharp
public PivotConditionFormatScopeType ScopeType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatPropertyScopeTypeDemo
    {
        public static void Run()
        {
            // Créez un classeur avec un tableau croisé dynamique
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Données d'exemple pour le tableau croisé dynamique
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(300);

            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ajoutez un format conditionnel au tableau croisé dynamique
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[formatIndex];
            pcf.ScopeType = PivotConditionFormatScopeType.Data;

            // Ajoutez une condition de format
            FormatConditionCollection fcs = pcf.FormatConditions;
            CellArea area = new CellArea();
            area.StartRow = 4;
            area.EndRow = 6;
            area.StartColumn = 5;
            area.EndColumn = 5;
            int[] conditionIndex = fcs.Add(area, FormatConditionType.CellValue, OperatorType.Between, "100", "200");
            
            // Définissez le style du format
            FormatCondition fc = fcs[conditionIndex[0]];
            fc.Style.BackgroundColor = Color.Yellow;

            // Enregistrez le classeur
            wb.Save("PivotConditionalFormatScopeTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotConditionFormatScopeType](../../pivotconditionformatscopetype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


