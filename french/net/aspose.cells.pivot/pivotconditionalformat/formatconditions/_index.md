---
title: "PivotConditionalFormat.FormatConditions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotConditionalFormat. Obtient les conditions pour le format conditionnel du tableau croisé"
type: docs
url: /fr/net/aspose.cells.pivot/pivotconditionalformat/formatconditions/
---
## PivotConditionalFormat.FormatConditions property

Obtenez les conditions du format conditionnel du tableau croisé dynamique.

```csharp
public FormatConditionCollection FormatConditions { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatPropertyFormatConditionsDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Créer des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 120;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 85;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 95;

            // Ajouter un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ajouter un format conditionnel
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivotTable.ConditionalFormats[formatIndex];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 1;
            area.EndRow = 3;
            area.EndColumn = 1;
            pfc.AddCellArea(area); // Apply to quantity column

            // Ajoutez une condition de format
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = pfc.FormatConditions[conditionIndex];
            fc.Formula1 = "100";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = System.Drawing.Color.Red;

            // Calculer les données du tableau croisé dynamique
            pivotTable.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotConditionalFormatExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [FormatConditionCollection](../../../aspose.cells/formatconditioncollection/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


