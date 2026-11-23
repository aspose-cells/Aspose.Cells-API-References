---
title: "Enum PivotConditionFormatRuleType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Pivot.PivotConditionFormatRuleType. Représente le type de règle de mise en forme conditionnelle du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivotconditionformatruletype/
---
## PivotConditionFormatRuleType enumeration

Représente le type de règle de mise en forme conditionnelle du **PivotTable**.

```csharp
public enum PivotConditionFormatRuleType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Indique que la mise en forme conditionnelle Top N n'est pas évaluée |
| All | `1` | Indique que la mise en forme conditionnelle Top N est évaluée sur l'ensemble de la plage de portée. |
| Row | `2` | Indique que la mise en forme conditionnelle Top N est évaluée pour chaque ligne. |
| Column | `3` | Indique que la mise en forme conditionnelle Top N est évaluée pour chaque colonne. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotConditionFormatRuleTypeDemo
    {
        public static void PivotConditionFormatRuleTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ajoutez des données d'exemple
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Ajouter un tableau croisé dynamique
            PivotTableCollection pivots = worksheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Ajouter PivotFormatCondition
            int formatIndex = pivot.PivotFormatConditions.Add();
            PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
            FormatConditionCollection fcc = pfc.FormatConditions;
            fcc.AddArea(pivot.DataBodyRange);
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "100";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = Color.Red;

            // Définir le type de règle pour le format conditionnel du tableau croisé dynamique
            pfc.RuleType = PivotConditionFormatRuleType.Row;

            // Actualiser et calculer les données du tableau croisé dynamique
            pivot.RefreshData();
            pivot.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotConditionFormatRuleTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


